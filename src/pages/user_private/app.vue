<template>
    <div>
        <footer class="mui-bar mui-bar-footer" id="cteate_btn">
            <button type="button" class="mui-btn mui-btn-hong-creat">创建练习赛</button>
        </footer>
        <div class="mui-content" id="pullrefresh">
            <div class="user_info">
                <div class="user_info_face">
                    <div id="face">
                        <!--<img src="../../assets/img/regbg_01.jpg"/>-->
                    </div>
                </div>
                <div class="manifesto mui-ellipsis">
                    小伙伴，搞起来！搞起来小伙伴，搞起来！搞起来小伙伴，搞起来！搞起来
                </div>
                <div class="user_info_msg">
                    <div class="user_name mui-pull-left">
                        <p id="userId">ID:1325786</p>
                        <p class="fontweight mui-ellipsis" id="userName">磨剪子抢菜刀磨剪子抢菜刀</p>
                    </div>
                    <div class="user_gamenum mui-pull-left">
                        <p>参赛场数</p>
                        <p class="fontweight" id="matchNum">120</p>
                    </div>
                    <div class="user_odds mui-pull-left">
                        <p>胜率</p>
                        <p class="fontweight" id="winRate">78%</p>
                    </div>
                </div>
                <div id="like_game">
                    <span class="dota"></span>
                    <span class="lol"></span>
                    <span class="fengbao"></span>
                    <span class="csgo"></span>
                </div>
                <div class="combat_values">
                    2312
                </div>
            </div>
            <div class="con">
                <div class="mui-segmented-control1">
                    <a class="mui-control-item1 mui-active" index=0>
                                我是选手
                            </a>
                    <a class="mui-control-item1" index=1>
                                我是OB
                            </a>
                </div>
                <div class="display_box">
                    <div class="mui-control-content1 active">
                        <div class="show_module">
                            <div class="module_title">我的战队</div>
                            <div class="module_con">
                                <div class="emptyToPlay">
                                    <span class="empty_logo">&nbsp;</span>
                                    <div class="ss">无战队,请
                                        <button type="button" class="mui-btn mui-btn-cheng-ty">创建战队</button> 或
                                        <button type="button" class="mui-btn mui-btn-green-jujue">加入其它战队</button>
                                    </div>
                                    <p>(每个用户一个游戏项目只能创建或者加入一个战队)</p>
                                </div>
                                <!--<div class="team_box">
                                            <div class="team_logo_box">
                                                <div class="team_logo">
                                                    <img src="../../assets/img/team_logo_03.jpg"/>
                                                </div>
                                                <div class="team_games">
                                                    <span class="dota"></span>
                                                </div>
                                            </div>
                                            <div class="team_ifno">
                                                <h4 class="mui-ellipsis">Mesut Ozil</h4>
                                                <p class="mui-ellipsis">小伙伴们！搞起来啊！快来啊搞起来啊！快来啊</p>
                                            </div>
                                            <div class="team_effectiveness">
                                                2341
                                            </div>
                                            <div class="team_btnbox">
                                                <button type="button" class="mui-btn mui-btn-cheng-ty">同意加入</button>
                
                                            </div>
                                        </div>
                                        <div class="team_box">
                                            <div class="team_logo_box">
                                                <div class="team_logo">
                                                    <img src="../../assets/img/team_logo_03.jpg"/>
                                                </div>
                                                <div class="team_games">
                                                    <span class="dota"></span>
                                                </div>
                                            </div>
                                            <div class="team_ifno">
                                                <h4 class="mui-ellipsis">Mesut Ozil</h4>
                                                <p class="mui-ellipsis">小伙伴们！搞起来啊！快来啊搞起来啊！快来啊</p>
                                            </div>
                                            <div class="team_effectiveness">
                                                2341
                                            </div>
                                            <div class="team_btnbox">
                                                <button type="button" class="mui-btn mui-btn-cheng-ty">同意加入</button>
                
                                            </div>
                                        </div>-->
    
                            </div>
    
                        </div>
                        <div class="show_module">
                            <div class="module_title">所在战队</div>
                            <div class="module_con">
                                <div class="team_box">
                                    <div class="team_logo_box">
                                        <div class="team_logo">
                                            <!--<img src="../../assets/img/dunpai_01.jpg"/>-->
                                        </div>
                                        <div class="team_games">
                                            <span class="dota"></span>
                                        </div>
                                    </div>
                                    <div class="team_ifno">
                                        <h4 class="mui-ellipsis">Mesut Ozil</h4>
                                        <p class="mui-ellipsis">小伙伴们！搞起来啊！快来啊搞起来啊！快来啊</p>
                                    </div>
                                    <div class="team_effectiveness">
                                        2341
                                    </div>
                                    <div class="team_btnbox">
                                        <button type="button" class="mui-btn mui-btn-green-jujue">同意加入</button>
                                        <!--<button type="button" class="mui-btn mui-btn-cheng">拒绝邀请</button>-->
                                    </div>
                                </div>
                                <div class="team_box">
                                    <div class="team_logo_box">
                                        <div class="team_logo">
                                            <img src="../../assets/img/team_logo_03.jpg" />
                                        </div>
                                        <div class="team_games">
                                            <span class="dota"></span>
                                        </div>
                                    </div>
                                    <div class="team_ifno">
                                        <h4 class="mui-ellipsis">Mesut Ozil</h4>
                                        <p class="mui-ellipsis">小伙伴们！搞起来啊！快来啊搞起来啊！快来啊</p>
                                    </div>
                                    <div class="team_effectiveness">
                                        2341
                                    </div>
                                    <div class="team_btnbox">
                                        <button type="button" class="mui-btn mui-btn-green-jujue">同意加入</button>
                                        <button type="button" class="mui-btn mui-btn-cheng-ty">拒绝邀请</button>
                                    </div>
                                </div>
                            </div>
    
                        </div>
                        <div class="show_module">
                            <div class="module_title">即将开始的比赛</div>
                            <div class="module_con">
                                <div class="tostartgame_box">
                                    <div class="tostartgame_con">
                                        <div class="team_logo">
                                            <div class="team_logo_box">
                                                <img src="../../assets/img/team_logo_03.jpg" />
                                            </div>
                                            <div class="team_name">
                                                TE-NAME
                                            </div>
                                        </div>
                                        <!-- <div class="game_score">2</div> -->
                                        <div class="team_vs">
                                            <div class="vs">vs</div>
                                            <div class="game_type">正赛</div>
                                            <div class="game_time">2.12 12：00</div>
                                        </div>
                                        <!-- <div class="game_score">1</div> -->
                                        <div class="team_logo">
                                            <div class="team_logo_box">
                                                <img src="../../assets/img/team_logo_03.jpg" />
                                            </div>
                                            <div class="team_name">
                                                TE-NAME
                                            </div>
                                        </div>
                                    </div>
                                    <!-- <div class="btn_box">
                                                <button type="button" class="mui-btn mui-btn-cheng-jieshou">接 受</button>
                                                <button type="button" class="mui-btn mui-btn-bai-jujue">拒 绝</button>
                                            </div> -->
                                </div>
                            </div>
                        </div>
                        <div class="show_module">
                            <div class="module_title">近期的比赛</div>
                            <div class="module_con">
                                <div class="minitostartgame_box">
                                    <div class="tostartgame_con">
                                        <div class="team_logo">
                                            <div class="team_logo_box">
                                                <img src="../../assets/img/team_logo_03.jpg" />
                                            </div>
    
                                        </div>
                                        <div class="game_score_left">
                                            <div class="team_name mui-ellipsis">
                                                TE-NAME
                                            </div>
                                            2
                                        </div>
                                        <div class="team_vs">
                                            <div class="game_type">正赛</div>
                                            <div class="game_time">2.12 12：00</div>
                                        </div>
                                        <div class="game_score_right">
                                            <div class="team_name mui-ellipsis">
                                                TE-NAME
                                            </div>
                                            1
                                        </div>
                                        <div class="team_logo">
                                            <div class="team_logo_box">
                                                <img src="../../assets/img/team_logo_03.jpg" />
                                            </div>
    
                                        </div>
                                    </div>
                                </div>
                                <div class="minitostartgame_box">
                                    <div class="tostartgame_con">
                                        <div class="team_logo">
                                            <div class="team_logo_box">
                                                <img src="../../assets/img/team_logo_03.jpg" />
                                            </div>
    
                                        </div>
                                        <div class="game_score_left">
                                            <div class="team_name mui-ellipsis">
                                                TE-NAME
                                            </div>
                                            2
                                        </div>
                                        <div class="team_vs">
                                            <div class="game_type">正赛</div>
                                            <div class="game_time">2.12 12：00</div>
                                        </div>
                                        <div class="game_score_right">
                                            <div class="team_name mui-ellipsis">
                                                TE-NAME
                                            </div>
                                            1
                                        </div>
                                        <div class="team_logo">
                                            <div class="team_logo_box">
                                                <img src="../../assets/img/team_logo_03.jpg" />
                                            </div>
    
                                        </div>
                                    </div>
                                </div>
                                <div class="minitostartgame_box">
                                    <div class="tostartgame_con">
                                        <div class="team_logo">
                                            <div class="team_logo_box">
                                                <img src="../../assets/img/team_logo_03.jpg" />
                                            </div>
    
                                        </div>
                                        <div class="game_score_left">
                                            <div class="team_name mui-ellipsis">
                                                TE-NAME
                                            </div>
                                            2
                                        </div>
                                        <div class="team_vs">
                                            <div class="game_type">正赛</div>
                                            <div class="game_time">2.12 12：00</div>
                                        </div>
                                        <div class="game_score_right">
                                            <div class="team_name mui-ellipsis">
                                                TE-NAME
                                            </div>
                                            1
                                        </div>
                                        <div class="team_logo">
                                            <div class="team_logo_box">
                                                <img src="../../assets/img/team_logo_03.jpg" />
                                            </div>
    
                                        </div>
                                    </div>
                                </div>
                                <div class="minitostartgame_box">
                                    <div class="tostartgame_con">
                                        <div class="team_logo">
                                            <div class="team_logo_box">
                                                <img src="../../assets/img/team_logo_03.jpg" />
                                            </div>
    
                                        </div>
                                        <div class="game_score_left">
                                            <div class="team_name mui-ellipsis">
                                                TE-NAME
                                            </div>
                                            2
                                        </div>
                                        <div class="team_vs">
                                            <div class="game_type">正赛</div>
                                            <div class="game_time">2.12 12：00</div>
                                        </div>
                                        <div class="game_score_right">
                                            <div class="team_name mui-ellipsis">
                                                TE-NAME
                                            </div>
                                            1
                                        </div>
                                        <div class="team_logo">
                                            <div class="team_logo_box">
                                                <img src="../../assets/img/team_logo_03.jpg" />
                                            </div>
    
                                        </div>
                                    </div>
                                </div>
                                <div class="minitostartgame_box">
                                    <div class="tostartgame_con">
                                        <div class="team_logo">
                                            <div class="team_logo_box">
                                                <img src="../../assets/img/team_logo_03.jpg" />
                                            </div>
                                        </div>
                                        <div class="game_score_left">
                                            <div class="team_name mui-ellipsis">
                                                TE-NAMETE-NAMETE-NAME
                                            </div>
                                            2
                                        </div>
                                        <div class="team_vs">
                                            <div class="game_type">正赛</div>
                                            <div class="game_time">2.12 12：00</div>
                                        </div>
                                        <div class="game_score_right">
                                            <div class="team_name mui-ellipsis">
                                                TE-NAME
                                            </div>
                                            1
                                        </div>
                                        <div class="team_logo">
                                            <div class="team_logo_box">
                                                <img src="../../assets/img/team_logo_03.jpg" />
                                            </div>
    
                                        </div>
                                    </div>
    
                                </div>
                            </div>
                            <div class="btn_box_width">
                                查看所有比赛历史
                            </div>
                        </div>
    
                    </div>
                    <div class="mui-control-content1">
                        <div class="show_module">
                            <div class="module_title">OB练习赛</div>
                            <div class="module_con">
                                <div class="tostartgame_box">
                                    <div class="tostartgame_con">
                                        <div class="team_logo">
                                            <div class="team_logo_box">
                                                <img src="../../assets/img/team_logo_03.jpg" />
                                            </div>
                                            <div class="team_name">
                                                TE-NAME
                                            </div>
                                        </div>
                                        <!--<div class="game_score">2</div>-->
                                        <div class="team_vs">
                                            <div class="vs">vs</div>
                                            <!--<div class="game_type">正赛</div>-->
                                            <div class="game_time">2.12 12：00</div>
                                        </div>
                                        <!--<div class="game_score">1</div>-->
                                        <div class="team_logo">
                                            <div class="team_logo_box">
                                                <img src="../../assets/img/team_logo_03.jpg" />
                                            </div>
                                            <div class="team_name">
                                                TE-NAME
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="show_module">
                            <div class="module_title">OB练习赛</div>
                            <div class="module_con">
                                <div class="tostartgame_box">
                                    <div class="tostartgame_con">
                                        <div class="team_logo">
                                            <div class="team_logo_box">
                                                <img src="../../assets/img/team_logo_03.jpg" />
                                            </div>
                                            <div class="team_name">
                                                TE-NAME
                                            </div>
                                        </div>
                                        <!--<div class="game_score">2</div>-->
                                        <div class="team_vs">
                                            <div class="vs">vs</div>
                                            <!--<div class="game_type">正赛</div>-->
                                            <div class="game_time">2.12 12：00</div>
                                        </div>
                                        <!--<div class="game_score">1</div>-->
                                        <div class="team_logo">
                                            <div class="team_logo_box">
                                                <img src="../../assets/img/team_logo_03.jpg" />
                                            </div>
                                            <div class="team_name">
                                                TE-NAME
                                            </div>
                                        </div>
                                    </div>
                                    <div class="btn_box">
                                        <button type="button" class="mui-btn mui-btn-cheng-jieshou">接 受</button>
                                        <button type="button" class="mui-btn mui-btn-bai-jujue">拒 绝</button>
                                    </div>
                                </div>
                            </div>
                            <div class="tostartgame_box">
                                <div class="tostartgame_con">
                                    <div class="team_logo">
                                        <div class="team_logo_box">
                                            <img src="../../assets/img/team_logo_03.jpg" />
                                        </div>
                                        <div class="team_name">
                                            TE-NAME
                                        </div>
                                    </div>
                                    <!--<div class="game_score">2</div>-->
                                    <div class="team_vs">
                                        <div class="vs">vs</div>
                                        <!--<div class="game_type">正赛</div>-->
                                        <div class="game_time">2.12 12：00</div>
                                    </div>
                                    <!--<div class="game_score">1</div>-->
                                    <div class="team_logo">
                                        <div class="team_logo_box">
                                            <img src="../../assets/img/team_logo_03.jpg" />
                                        </div>
                                        <div class="team_name">
                                            TE-NAME
                                        </div>
                                    </div>
                                </div>
                                <div class="btn_box">
                                    <button type="button" class="mui-btn mui-btn-cheng-jieshou">接 受</button>
                                    <button type="button" class="mui-btn mui-btn-bai-jujue">拒 绝</button>
                                </div>
                            </div>
                        </div>
                        <div class="show_module">
                            <div class="module_title">OB历史</div>
                            <div class="module_con">
                                <div class="minitostartgame_box">
                                    <div class="tostartgame_con">
                                        <div class="team_logo">
                                            <div class="team_logo_box">
                                                <img src="../../assets/img/team_logo_03.jpg" />
                                            </div>
    
                                        </div>
                                        <div class="game_score_left">
                                            <div class="team_name mui-ellipsis">
                                                TE-NAME
                                            </div>
                                            2
                                        </div>
                                        <div class="team_vs">
                                            <div class="game_type">正赛</div>
                                            <div class="game_time">2.12 12：00</div>
                                        </div>
                                        <div class="game_score_right">
                                            <div class="team_name mui-ellipsis">
                                                TE-NAME
                                            </div>
                                            1
                                        </div>
                                        <div class="team_logo">
                                            <div class="team_logo_box">
                                                <img src="../../assets/img/team_logo_03.jpg" />
                                            </div>
    
                                        </div>
                                    </div>
                                </div>
                                <div class="minitostartgame_box">
                                    <div class="tostartgame_con">
                                        <div class="team_logo">
                                            <div class="team_logo_box">
                                                <img src="../../assets/img/team_logo_03.jpg" />
                                            </div>
    
                                        </div>
                                        <div class="game_score_left">
                                            <div class="team_name mui-ellipsis">
                                                TE-NAME
                                            </div>
                                            2
                                        </div>
                                        <div class="team_vs">
                                            <div class="game_type">正赛</div>
                                            <div class="game_time">2.12 12：00</div>
                                        </div>
                                        <div class="game_score_right">
                                            <div class="team_name mui-ellipsis">
                                                TE-NAME
                                            </div>
                                            1
                                        </div>
                                        <div class="team_logo">
                                            <div class="team_logo_box">
                                                <img src="../../assets/img/team_logo_03.jpg" />
                                            </div>
    
                                        </div>
                                    </div>
                                </div>
                                <div class="minitostartgame_box">
                                    <div class="tostartgame_con">
                                        <div class="team_logo">
                                            <div class="team_logo_box">
                                                <img src="../../assets/img/team_logo_03.jpg" />
                                            </div>
    
                                        </div>
                                        <div class="game_score_left">
                                            <div class="team_name mui-ellipsis">
                                                TE-NAME
                                            </div>
                                            2
                                        </div>
                                        <div class="team_vs">
                                            <div class="game_type">正赛</div>
                                            <div class="game_time">2.12 12：00</div>
                                        </div>
                                        <div class="game_score_right">
                                            <div class="team_name mui-ellipsis">
                                                TE-NAME
                                            </div>
                                            1
                                        </div>
                                        <div class="team_logo">
                                            <div class="team_logo_box">
                                                <img src="../../assets/img/team_logo_03.jpg" />
                                            </div>
    
                                        </div>
                                    </div>
                                </div>
                                <div class="minitostartgame_box">
                                    <div class="tostartgame_con">
                                        <div class="team_logo">
                                            <div class="team_logo_box">
                                                <img src="../../assets/img/team_logo_03.jpg" />
                                            </div>
    
                                        </div>
                                        <div class="game_score_left">
                                            <div class="team_name mui-ellipsis">
                                                TE-NAME
                                            </div>
                                            2
                                        </div>
                                        <div class="team_vs">
                                            <div class="game_type">正赛</div>
                                            <div class="game_time">2.12 12：00</div>
                                        </div>
                                        <div class="game_score_right">
                                            <div class="team_name mui-ellipsis">
                                                TE-NAME
                                            </div>
                                            1
                                        </div>
                                        <div class="team_logo">
                                            <div class="team_logo_box">
                                                <img src="../../assets/img/team_logo_03.jpg" />
                                            </div>
    
                                        </div>
                                    </div>
                                </div>
                                <div class="minitostartgame_box">
                                    <div class="tostartgame_con">
                                        <div class="team_logo">
                                            <div class="team_logo_box">
                                                <img src="../../assets/img/team_logo_03.jpg" />
                                            </div>
                                        </div>
                                        <div class="game_score_left">
                                            <div class="team_name mui-ellipsis">
                                                TE-NAMETE-NAMETE-NAME
                                            </div>
                                            2
                                        </div>
                                        <div class="team_vs">
                                            <div class="game_type">正赛</div>
                                            <div class="game_time">2.12 12：00</div>
                                        </div>
                                        <div class="game_score_right">
                                            <div class="team_name mui-ellipsis">
                                                TE-NAME
                                            </div>
                                            1
                                        </div>
                                        <div class="team_logo">
                                            <div class="team_logo_box">
                                                <img src="../../assets/img/team_logo_03.jpg" />
                                            </div>
                                        </div>
                                    </div>
    
                                </div>
                            </div>
                            <div class="btn_box_width">
                                查看所有比赛历史
                            </div>
                        </div>
                    </div>
                </div>
    
            </div>
        </div>
    </div>
</template>

<script>
require("expose-loader?mui!assets/js/mui.js");
import { app } from 'assets/js/appp.js';
mui.init();
mui.plusReady(function () {
    var cteate_btn = document.getElementById('cteate_btn');
    mui('.mui-segmented-control1').on('tap', '.mui-control-item1', function () {
        var index = this.getAttribute('index') - 0;
        mui('.mui-control-item1').each(function () {
            this.classList.remove('mui-active');
        });
        this.classList.add('mui-active');
        mui('.mui-control-content1').each(function () {
            this.classList.remove('active');
        });
        mui('.mui-control-content1')[index].classList.add('active');
        cteate_btn.classList.remove('show');
        if (index) {
            cteate_btn.classList.add('show');
        }

    });
    mui('.mui-bar-footer').on('tap', '.mui-btn-hong-creat', function () {
        mui.openWindow({
            url: "../create_lianxi_match.html",
            id: "create_lianxi_match.html",
            preload: true,

        })
    });


});



export default {}
</script>

<style>

</style>
