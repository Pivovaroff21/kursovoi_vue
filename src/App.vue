<template>
   <header>
      <div class="text_block">
        <div class="wrapper">
          <i class="fa-solid fa-phone"></i>
          <span class="contact_phone">050 080 50 49</span>
        </div>
      </div>
      <div class="logo_block">
        <div class="wrapper">
          <router-link to="/" class="logo_link">
            <span class="logo_text">PAYBOX</span>
          </router-link>
        </div>
      </div>
    </header>
    <router-view></router-view>
</template>

<script>
export default {
  name:"App",
}

</script>

<style>


html {
  box-sizing: border-box;
}

body{
  box-sizing: border-box;
  font-family: "Roboto", serif;
  font-size: normal;
  font-weight: 500;
  font-size: 18px;
  line-height: 1.2em;
  background-color:  #fdfbfc ;
}

img {
  max-width: 100%;
  height: auto;
}




/* operator styles*/

.wrapper{
    max-width: 1370px;
    margin:0 auto;
}

.operator_cards_wrap{
    padding:0px 15px;
    height:100vh;
    display:flex;
    align-items: center;
    justify-content: space-between;
}





.operator_card{
    flex: 1 0 0;
    height: 200px;
    width:450px;
    border-radius: 9px;
    border: 1px solid rgba(125,125,125,.27);
    transition: all .57s cubic-bezier(0,0,.58,1);
    padding:50px ;
    background-color:#fff;

}

.operator_card:hover{
    border-color:rgba(225,76,154,.46);
    box-shadow:0 37px 30px -34px rgba(225,76,154,.46);
    transition:all .2s ease-in-out;
}

.operator_card:hover .operator_name{
    color:#e14c9a;
    transition: .5s ;
}
.operator_name{
    font-size: 48px;
    line-height: 62px;
    font-family: "Roboto",sans-serif;
    padding-top: 57px;
    text-align: center;
    color: #7d7d7d;

}

.tariff_operator_name{
    margin-bottom: 50px;
}

.operator_link{
    text-decoration: none;
}
/*operator styles ends*/

/* tariff styles start*/

.tariff_card{
    width: 200px;
    font-weight: 400;
    font-size: 18px;
    line-height: 24px;
    min-height: 200px;
    border-radius: 9px;
    border: 1px solid rgba(125,125,125,.27);
    transition: all .57s cubic-bezier(0,0,.58,1);
    padding:20px ;
    background-color:#fff;
}

.tariff_cards_wrap{
    display:flex;
    flex-wrap: wrap;
    justify-content: space-evenly;
    color: #7d7d7d;
}
.tariff_cost{
    font-size: 20px;
    font-weight: 700;
    margin-bottom: 10px;
    color: #000;

}

.tariff_desc{
    margin-bottom:10px;
}

.tariff_link{
    display: block;
    max-width: 140px;
    margin:0 auto;
    text-decoration: none;
    border-radius: 25px;
    background-image: -webkit-linear-gradient(-136deg,#f28cb2 0,#f172a0 47%,#f24a88 100%);
    cursor: pointer;
    color:#fff;
    padding: 20px;
    transition: 0.25s;
    text-align: center;
    border-color:transparent;
}

.tariff_link:hover{
    opacity:0.7;
}

.tariff_name{
    font-size: 20px;
    margin-bottom: 10px;
}


/* phone_input_form styles*/

.wrapper_form{
    max-width: 1370px;
    margin: 0 auto;
    display: flex;
    justify-content:space-between;
    margin-top: 100px;
}

.tips{
    font-size: 16px;
    padding: 50px 50px 20px;
    max-width: 330px;
    border-radius: 9px;
    margin-bottom: 70px;
    background-color: #fefefe;
    text-align: left;
    box-shadow: 0 0 21px rgb(0 0 0 / 16%);
}
.tips_text{
    font-size: 18px;
    margin-bottom: 20px;
}

.tips_list{
    padding-left: 30px;
    margin-bottom: 20px;
}

.tips_list_item{
    margin-bottom: 10px;
}

.img_wrap{
    width:300px;
    margin:0 auto;
}
.tip_block_pic{
    height: 245px;

}

.tips_list_item::before{
    content: "\2022";
    color: #e14c9a;
    font-weight: 700;
    display: inline-block;
    width: 1em;
    font-size: 25px;
    line-height: 1.5rem;
}


.phone_form{
    display: flex;
    flex-direction: column;
    padding: 40px 70px 0;
    border-radius: 9px;
    box-shadow: 0 0 30px -8px rgb(225 76 154 / 46%);
    margin-bottom: 20px;
    width: 505px;
    min-height: 560px;
    background-color:#fff;
}

.phone_form_input{
    width: 70%;
    mix-blend-mode: normal;
    border: none;
    border-bottom: 1px solid rgba(125,125,125,.5);
    border-radius: 0;
    outline: 0;
    font-weight: 500;
    font-size: 24px;
    line-height: 29px;
    letter-spacing: .3px;
    color: #343434;
    margin-bottom: 50px;

}

.form_input_first{
    padding-left: 55px;
    margin-bottom: 10px;

}



.phone_input_wrap{
    position: relative;
}

.Kyivstar::after , .Vodafone::after, .Lifecell::after{
    content: "";
    width: 50px;
    height: 50px;
    top: -15px;
    right: 45px;
    position: absolute;
    display: inline-block;

}

/* .Kyivstar::after{
     background: url(../img/1.png);
}
.Vodafone::after{
    background: url(../img/2.png);
}
.Lifecell::after{
    background: url(../img/3.png);
} */


.phone_input_wrap::before{
    content:"+380";
    font-size: 24px;
    line-height: 29px;
    letter-spacing: .3px;
    color: #343434;
    width:50px;
    position: absolute;
    top:1px;
}

.error{

    display: none;
    color:red;
    max-width: 82%;
    font-size: 16px;
    line-height: 22px;
}



.form_input_last{
    margin-bottom: 20px;
    width: 80.5%;
}


.phone_form_text{
    font-size: 18px;
    font-family: "Roboto",sans-serif;
    margin-bottom: 20px;
    color: #7d7d7d;
}



.subtitle_name{
    font-size: 32px;
    line-height: 48px;
    font-family: "Roboto",sans-serif;
    text-align: center;
    color: #7d7d7d;
    margin-bottom: 20px;
}

.value_buttons{
    width: 50%;
    display: flex;
    justify-content: space-between;
    margin-bottom: 20px;
    text-decoration: underline;
}

.value_but{
    transition: .25s;
    cursor: pointer;
}

.value_but:hover{
    opacity: 0.5;
}




/*header*/

.text_block{
    height: 61px;
    background-color: #3d4040;

}

.logo_block{
    height: 82px;
    background-color: #fff;
    box-shadow: 0 3px 6px -2px rgb(225 76 154 / 30%);
}

.fa-phone{
    color:#FFF;
    padding-top: 20px;
}

.contact_phone{
    color:#fff;
    font-size: 16px;
    font-weight: 700;
    letter-spacing: .5px;
    margin-left: 25px       ;
}

.logo_text{
    display: inline-block;
    font-size: 32px;
    line-height: 48px;
    color:#e14c9a;
    font-weight: 900;
    padding-top: 15px;

}

.logo_link{
    transition: .25s;
    text-decoration: none;
}
.logo_text:hover{
    opacity:0.5;
}
/*transaction styles*/
.transaction{
    margin:0 auto;
    margin-top: 100px;
    padding: 50px 50px 20px;
    max-width: 720px;
    min-height: 500px;
    border-radius: 9px;
    margin-bottom: 70px;
    background-color: #fefefe;
    text-align: left;
    box-shadow: 0 0 21px rgb(0 0 0 / 16%);
}

.transactio_inner{
    padding: 175px;
    text-align: center;
}

.transaction_id{
    font-size: 32px;
    line-height: 48px;
    font-weight: 700;
    margin-bottom: 10px;
}

.transaction_text{
    color:green;
}

.transaction_text_red{
    color:red;
}

</style>