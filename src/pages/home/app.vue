<template>
  <div id="app">
     <header class="mui-bar mui-bar-nav">
      <a id="search_btn" class="mui-icon mui-icon-search mui-pull-right"></a>
      <a id="setting" class="mui-icon mui-icon-gear-filled mui-pull-right"></a>
      <a id="creat_team_btn" class="mui-icon mui-pull-right creat_team">创建战队</a>
      <h1 class="mui-title" id="title">个人中心</h1>
    </header>
    <nav class="mui-bar mui-bar-tab">
        <a class="mui-tab-item" href="html/msg.html">
            <span class="gaoqi-icon gaoqi-icon-msg" style="top: 5px;"><span
                    class="mui-badge mui-badge-danger"></span></span>
            <span class="mui-tab-label">消息</span>
        </a>
        <a class="mui-tab-item" href="html/friend.html">
            <span class="gaoqi-icon gaoqi-icon-hb"></span>
            <span class="mui-tab-label">伙伴</span>
        </a>
        <a id="defaultTab" class="mui-tab-item mui-active" href="html/user_private.html">
            <span class="gaoqi-icon gaoqi-icon-me"></span>
            <span class="mui-tab-label">我的</span>
        </a>
        <a class="mui-tab-item" href="match.html">
            <span class="gaoqi-icon gaoqi-icon-ss"></span>
            <span class="mui-tab-label">赛事</span>
        </a>
        <a class="mui-tab-item" href="html/team.html">
            <span class="gaoqi-icon gaoqi-icon-zd"></span>
            <span class="mui-tab-label">战队</span>
        </a>
    </nav>
  </div>

</template>

<script>
export default {
  
}

import mui from 'assets/js/mui.min.js';
    //mui初始化
    mui.init();
    var subpages = ['html/user_private.html', 'html/friend.html', 'match.html', 'html/msg.html', 'html/team.html'];
    var subpage_style = {
        top: '44px',
        bottom: '51px'
    };

    var aniShow = {};
    var btnArray = document.querySelectorAll('.mui-bar-nav a');
    /************************************************************************/
    /* 创建子页面，首个选项卡页面显示，其它均隐藏；                             */
    /************************************************************************/
    mui.plusReady(function () {
        var self = plus.webview.currentWebview();
        var btnArray = document.querySelectorAll('.mui-bar-nav a');
        for (var i = 0; i < 5; i++) {
            var temp = {};
            var sub = plus.webview.create(subpages[i], subpages[i], subpage_style);
            if (i > 0) {
                sub.hide();
            } else {
                temp[subpages[i]] = "true";
                mui.extend(aniShow, temp);
            }
            self.append(sub);
        }
        
        btnArray[0].style.display = 'none';
        btnArray[1].style.display = 'block';
        btnArray[2].style.display = 'none';
        //点击设置按钮打开设置页面
        document.querySelector('#setting').addEventListener('tap', function () {
            mui.openWindow({
                url: "html/setting.html",
                id: "setting",
                preload: true,
                show: {
                    aniShow: 'pop-in'
                }
            })
        });

        /************************************************************************/
        /*激活当前选项卡                                                          */
        /************************************************************************/
        var activeTab = subpages[0];
        var title = document.getElementById("title");

        //选项卡点击事件
        mui('.mui-bar-tab').on('tap', 'a', function (e) {

            var targetTab = this.getAttribute('href');
            //更换标题
            title.innerHTML = this.querySelector('.mui-tab-label').innerHTML;
            //更换右上角搜索 创建战队 设置的按钮
            if (targetTab === 'html/team.html') {
                btnArray[0].style.display = 'block';
                btnArray[1].style.display = 'none';
                btnArray[2].style.display = 'block';
            } else if (targetTab === 'html/user_private.html') {
                btnArray[0].style.display = 'none';
                btnArray[1].style.display = 'block';
                btnArray[2].style.display = 'none';
            } else {
                btnArray[0].style.display = 'block';
                btnArray[1].style.display = 'none';
                btnArray[2].style.display = 'none';
            }
            if (targetTab === activeTab) {
                return;
            }

            //显示目标选项卡
            //若为iOS平台或非首次显示，则直接显示
            if (mui.os.ios || aniShow[targetTab]) {
                plus.webview.show(targetTab);
            } else {
                //否则，使用fade-in动画，且保存变量
                var temp = {};
                temp[targetTab] = "true";
                mui.extend(aniShow, temp);
                plus.webview.show(targetTab, "fade-in", 300);
            }
            //隐藏当前;
            plus.webview.hide(activeTab);
            //更改当前活跃的选项卡
            activeTab = targetTab;
        });
        //自定义事件，模拟点击“首页选项卡”
        document.addEventListener('gohome', function () {
            var defaultTab = document.getElementById("defaultTab");
            //模拟首页点击
            mui.trigger(defaultTab, 'tap');
            //切换选项卡高亮
            var current = document.querySelector(".mui-bar-tab>.mui-tab-item.mui-active");
            if (defaultTab !== current) {
                current.classList.remove('mui-active');
                defaultTab.classList.add('mui-active');
            }
        });
        //禁止返回按钮
        //
        mui.oldBack = mui.back;
        var backButtonPress = 0;
        mui.back = function (event) {
            backButtonPress++;
            if (backButtonPress > 1) {
                plus.runtime.quit();
            } else {
                plus.nativeUI.toast('再按一次退出应用');
            }
            setTimeout(function () {
                backButtonPress = 0;
            }, 1000);
            return false;
        };

        //增加首页刷新时间
    });
</script>

<style lang="css">
 .mui-bar-nav.mui-bar .mui-icon.creat_team {
            font-size: 14px !important;
            line-height: 27px;
        }

        #search_btn {
            display: none;
        }

        #creat_team_btn {
            display: none;
        }
</style>
