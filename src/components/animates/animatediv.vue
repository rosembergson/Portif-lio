<template>
<div>
    <div class="animatediv_bg">
        <div class="animatediv_container">
            <h2> Rosembergson Lacerda </h2>
            <div class="container--divshow">
                <div class="container--divshow--1"> 
                    <h4> Quem é Rosembergson Lacerda </h4>
                    <p>Graduando em Redes de Computadores que trabalha atualmente com desenvolvimento frontend na empresa 
                        OSF Global Services. Tecnologias com Vue.js e com começo em Angular.js .
                        É iniciante na área de projeto, porém busca sempre da seu melhor na feição de tais projetos.
                    </p>
                    <button type="button">Biografia</button>
                </div>
                <div class="container--divshow--2"> 
                    <div class="flip-box">
                        <div class="flip-box-inner">
                             <div class="flip-box-front">
                                
                             </div>
                             <div class="flip-box-back">
                                <form class="div_animate_1"> 
                                    <label for="name"> Name : <input type="text" name="name" ></label>
                                    <label for="email"> Email : <input type="email" name="email" ></label>
                                    <label for="idade"> Idade : <input type="text" name="idade" ></label>
                                    <button type="button"> Enviar </button>
                                </form>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss">
    @import '../../scss/animatediv.scss';
    @import '../../scss/animationcard.scss'
</style>
