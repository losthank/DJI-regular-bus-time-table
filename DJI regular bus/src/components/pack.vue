<template>
  <div id="app">
<section id = 'bbox'>
<section class="box">
  <h2>粤BCZ158</h2>
<table>
  <tr>
    <td v-for="item in items1">{{item.name}}</td>
  </tr>
   <tr>
    <td v-for="item in times1">{{item.time}}</td>
  </tr>
</table>
<table>
  <tr>
    <td v-for="item in items2">{{item.name}}</td>
  </tr>
   <tr>
    <td v-for="item in times2">{{item.time}}</td>
  </tr>
</table>
</section>
</br>
<section class="box">
  <h2>粤BAV996</h2>
<table>
  <tr>
    <td v-for="item in items3">{{item.name}}</td>
  </tr>
   <tr>
    <td v-for="item in times3">{{item.time}}</td>
  </tr>
</table>
<table>
  <tr>
    <td v-for="item in items4">{{item.name}}</td>
  </tr>
   <tr>
    <td v-for="item in times4">{{item.time}}</td>
  </tr>
</table>
</section>
</br>
<section class="box">
  <h2>粤N9K42</h2>
<table>
  <tr>
    <td v-for="item in items5">{{item.name}}</td>
  </tr>
   <tr>
    <td v-for="item in times5">{{item.time}}</td>
  </tr>
</table>
<table>
  <tr>
    <td v-for="item in items6">{{item.name}}</td>
  </tr>
   <tr>
    <td v-for="item in times6">{{item.time}}</td>
  </tr>
</table>
</section>
<br>
<section class="box">
  <h2>粤BW1761</h2>
<table>
  <tr>
    <td v-for="item in items7">{{item.name}}</td>
  </tr>
   <tr>
    <td v-for="item in times7">{{item.time}}</td>
  </tr>
</table>
<table>
  <tr>
    <td v-for="item in items8">{{item.name}}</td>
  </tr>
   <tr>
    <td v-for="item in times8">{{item.time}}</td>
  </tr>
</table>
</section>
</section>

<aside id="note">
  注意：<br>
  1、仅供文件、物品的托运，不可搭乘人员；<br>
  2、表格所标注时间为各地点发车时间；<br>
  3、班车准时出发，如需使用班车传递物品，请于发车前20分钟，将物品寄放在收发货的位置。<br>
  大件物品需自行送至发车地点（大件物品：累计重量超过10KG或体积超过0.08立方米的物品）<br>
  <aside id="position">
  <table>
    <tr><th>发车地点</th><th>收发货位置</th></tr>
    <tr><td>创维西座B1层</td><td>14F收发室</td></tr>
    <tr><td>创维东座B1层</td><td>5F收发室</td></tr>
    <tr><td>威新7栋1F南门</td><td>7栋6F收发室</td></tr>
    <tr><td>宝安工厂2号门</td><td>1F收发室</td></tr>
    <tr><td>百旺工厂7栋1F</td><td>7栋1F收发室</td></tr>
    <tr><td>石岩29号收货台</td><td>29号收货台</td></tr>
    <tr><td>集成电路1F正门</td><td>2F前台</td></tr>
    <tr><td>百旺信11栋</td><td>1F收发区</td></tr>
    <tr><td>百旺信13栋</td><td>5F收发室</td></tr>
    <tr><td>南山云谷</td><td>6F收发室</td></tr>
    <tr><td>欢乐海岸</td><td>旗舰店</td></tr>
    <tr><td>科大6F</td><td>6F收发室</td></tr>
  </table>
</aside>
</aside>


  </div>
</template>

<script>
export default{
  data(){
    return {
      items1:[
        {name:'路线1'},
        {name:'创维西座'},
        {name:'威新'},
        {name:'石岩成品仓'},
        {name:'百旺信（13栋）'},  
        {name:' 百旺信（11栋）'},
        {name:'百旺工厂'},
        {name:'创维西座'},
      ],
      times1:[
        {time:''},
        {time:'9:00'},
        {time:'9:20'},
        {time:'10:20'},
        {time:'10:50'},
        {time:'11:00'},
        {time:'11:30'},
        {time:'-'}
      ],
      items2:[
        {name:'路线2'},
        {name:'创维西座'},
        {name:'威新'},
        {name:'集成电路'},
        {name:'石岩成品仓'},  
        {name:' 百旺工厂'},
        {name:'百旺信（13栋）'},
        {name:'百旺信（11栋）'},
        {name:'威新'},
        {name:'创维西座'},
      ],
      times2:[
        {time:''},
        {time:'14:20'},
        {time:'14:40'},
        {time:'15:00'},
        {time:'15:45'},
        {time:'16:20'},
        {time:'17:00'},
        {time:'17:10'},
        {time:'17:40'},
        {time:'-'}
      ],

            items3:[
        {name:'路线1'},
        {name:'百旺信（11栋）'},
        {name:'百旺信（13栋）'},
        {name:'百旺工厂'},
        {name:'集成电路'},  
        {name:'威新'},
        {name:'创维西座'},
        {name:'威新'},
        {name:'百旺信（13栋）'}
      ],
      times3:[
        {time:''},
        {time:'9:00'},
        {time:'9:10'},
        {time:'9:30'},
        {time:'10:00'},
        {time:'10:30'},
        {time:'11:20'},
        {time:'11:40'},
        {time:'-'}
      ],
            items4:[
        {name:'路线2'},
        {name:'百旺信（11栋）'},
        {name:'百旺信（13栋）'},
        {name:'百旺工厂'},
        {name:'集成电路'},  
        {name:'威新'},
        {name:'创维西座'},
        {name:'威新'},
        {name:'百旺信（13栋）'},
        {name:'百旺'}
      ],
      times4:[
        {time:''},
        {time:'14:00'},
        {time:'14:10'},
        {time:'14:30'},
        {time:'15:00'},
        {time:'15:40'},
        {time:'16:20'},
        {time:'16:40'},
        {time:'17:30'},
        {time:'-'}
      ],

            items5:[
        {name:'路线1'},
        {name:'科大'},
        {name:'宝安工厂'},
        {name:'集成电路'},  
        {name:'南山云谷'},
        {name:'百旺信（11栋）'},
        {name:'南山云谷'},
        {name:'科大'}
      ],
      times5:[
        {time:''},
        {time:'9:05'},
        {time:'9:30'},
        {time:'10:00'},
        {time:'10:30'},
        {time:'11:00'},
        {time:'11:30'},
        {time:'-'}
      ],
            items6:[
        {name:'路线2'},
        {name:'科大'},
        {name:'欢乐海岸'},
        {name:'集成电路'},  
        {name:'南山云谷'},
        {name:'百旺信（11栋）'},
        {name:'欢乐海岸'},
        {name:'科大'},
      ],
      times6:[
        {time:''},
        {time:'14:00'},
        {time:'14:20'},
        {time:'15:00'},
        {time:'15:30'},
        {time:'16:10'},
        {time:'16:40'},
        {time:'-'}
      ],

      items7:[
        {name:'路线1'},
        {name:'百旺工厂'},
        {name:'百旺信工厂'}
      ],
      times7:[
        {time:''},
        {time:'10:30'},
        {time:'11:10'}
      ],
            items8:[
        {name:'路线2'},
{name:'百旺工厂'},
{name:'百旺信工厂'},
{name:'百旺工厂'},
{name:'百旺信工厂'}
      ],
      times8:[
        {time:''},
        {time:'15:15'},
        {time:'15:55'},
        {time:'16:35'},
        {time:'17:15'}
      ],
    }
  }
}
</script>

<style scoped>
#bbox{
  display:inline-block;
    margin:0 auto;
    margin-top:-60px;
}
.box table{
  border:1px black solid;
}
.box table td{
  width:125px;
  padding-bottom:6px;
}
.box table td:first-child{color:#2eaced;font-size: 1.2em;}
#note{
float: left;
text-align: left;
width: 500px;
background-color: #d9f7f2;
padding-top:8px;
margin-top: 20px;
}
#position{
  margin-top:50px;
}
#position table td{
  border: 1px grey solid;
}
#position table th td{
  border: 1px grey solid;

}
#position table{
   border-collapse: collapse;
}

</style>