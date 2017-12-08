<template>
  <div id="app">
  <section id = 'bbox'>
  <h2>创维-威新</h2>
<table>
  <tr>
    <td v-for="item in time1">{{item.time}}</td>
  </tr>
   <tr>
    <td v-for="item in car1">{{item.name}}</td>
  </tr>
</table>
<h2>威新-创维</h2>
<table>
  <tr>
    <td v-for="item in time2">{{item.time}}</td>
  </tr>
   <tr>
    <td v-for="item in car1">{{item.name}}</td>
  </tr>
</table>

  <aside id="note">
  注意：<br>
  1、仅供人员搭乘，不可托运货物，班车搭乘遵循先到先得；<br>
  2、表格所标注时间为各地点发车时间；<br>
  3、请于发车前10分钟，在班车所在办公地的指定地点。
  <aside id="position">
  <table>
    <tr><th>发车地点</th><th>乘车位置</th></tr>
    <tr><td>创维</td><td>西座B1层</td></tr>
    
    <tr><td>威新</td><td>7栋一楼南门</td></tr>
    <tr><td>集成电路1F正门</td><td>2F前台</td></tr>
    <tr><td>百旺工厂</td><td>7栋一楼前台宣传栏对面</td></tr>
    <tr><td>百旺信</td><td>13栋一楼南门</td></tr>
  </table>
</aside>
</aside>

<h2>创维-百旺工厂</h2>
<table>
  <tr>
    <td v-for="item in time3">{{item.time}}</td>
  </tr>
   <tr>
    <td v-for="item in car3">{{item.name}}</td>
  </tr>
</table>
<h2>百旺工厂-创维</h2>
<table>
  <tr>
    <td v-for="item in time4">{{item.time}}</td>
  </tr>
   <tr>
    <td v-for="item in car4">{{item.name}}</td>
  </tr>
</table>
<h2>创维-百旺信</h2>
<table>
  <tr>
    <td v-for="item in time4">{{item.time}}</td>
  </tr>
   <tr>
    <td v-for="item in car3">{{item.name}}</td>
  </tr>
</table>


<h2>百旺信-创维</h2>
<table>
  <tr>
    <td v-for="item in time6">{{item.time}}</td>
  </tr>
   <tr>
    <td v-for="item in car6">{{item.name}}</td>
  </tr>
</table>
<h2>百旺信-百旺工厂</h2>
<table>
  <tr>
    <td v-for="item in time7">{{item.time}}</td>
  </tr>
   <tr>
    <td v-for="item in car7">{{item.name}}</td>
  </tr>
</table>
<h2>百旺工厂-百旺信</h2>
<table>
  <tr>
    <td v-for="item in time8">{{item.time}}</td>
  </tr>
   <tr>
    <td v-for="item in car8">{{item.name}}</td>
  </tr>
</table>


</section>



  </div>
</template>

<script>
export default{
  data(){
    return {
      time1:[
          {time:'时间'},
        {time:'9:00'},
        {time:'9:40'},
        {time:'10:20'},
        {time:'10:50'},
        {time:'11:00'},
        {time:'11:40'},
        {time:'11:50'},
        {time:'12:15'},
        {time:'14:00'},
        {time:'14:40'},
        {time:'15:20'},
        {time:'15:30'},
        {time:'16:00'},
        {time:'16:30'},
        {time:'16:40'},
        {time:'17:20'}
      ],
      car1:[
         {name:'车辆'},
        {name:'3号车'},
        {name:'3号车'},
        {name:'3号车'},
        {name:'2号车'},
        {name:'3号车'},
        {name:'3号车'},
        {name:'1号车'},
        {name:'3号车'},
        {name:'3号车'},
        {name:'3号车'},
        {name:'3号车'},
        {name:'1号车'},
        {name:'3号车'},
        {name:'2号车'},
        {name:'3号车'},
        {name:'3号车'}
      ],
      time2:[
        {time:'时间'},
        {time:'9:20'},
        {time:'10:00'},
        {time:'10:40'},
        {time:'11:10'},
        {time:'11:20'},
        {time:'12:00'},
        {time:'12:10'},
        {time:'12:25'},
        {time:'14:20'},
        {time:'15:00'},
        {time:'15:40'},
        {time:'15:50'},
        {time:'16:20'},
        {time:'16:50'},
        {time:'17:00'},
        {time:'17:40'}
      ],//车号同上
time3:[
          {time:'时间'},
        {time:'9:00'},
        {time:'9:30'},
        {time:'10:30'},
        {time:'11:30'},
        {time:'14:15'},
        {time:'14:50'},
        {time:'16:10'},
        {time:'17:20'}
      ],
      car3:[
         {name:'车辆'},
        {name:'1号车'},
        {name:'2号车'},
        {name:'1号车'},
        {name:'2号车'},
        {name:'1号车'},
        {name:'2号车'},
        {name:'1号车'},
        {name:'2号车'},
      ],
      time4:[
          {time:'时间'},
        {time:'8:40'},
        {time:'9:50'},
        {time:'10:10'},
        {time:'11:10'},
        {time:'14:10'},
        {time:'14:50'},
        {time:'15:40'},
        {time:'17:20'}
      ],
      car4:[
         {name:'车辆'},
        {name:'2号车'},
        {name:'1号车'},
        {name:'2号车'},
        {name:'1号车'},
        {name:'2号车'},
        {name:'1号车'},
        {name:'2号车'},
        {name:'1号车'}
      ],//时间同上4 车辆同上3
    time6:[
          {time:'时间'},
        {time:'9:35'},
        {time:'10:00'},
        {time:'11:05'},
        {time:'14:05'},
        {time:'14:45'},
        {time:'15:30'},
        {time:'16:55'}
      ],
      car6:[
         {name:'车辆'},
        {name:'1号车'},
        {name:'2号车'},
        {name:'1号车'},
        {name:'2号车'},
        {name:'1号车'},
        {name:'2号车'},
        {name:'1号车'},
      ],
          time7:[
          {time:'时间'},
    {time:'9:35'},
        {time:'10:00'},
        {time:'11:05'},
        {time:'11:10'},
        {time:'14:05'},
        {time:'14:45'},
        {time:'15:30'},
        {time:'15:55'},
        {time:'16:55'},
        {time:'17:15'}
      ],
           car7:[
         {name:'车辆'},
        {name:'1号车'},
        {name:'2号车'},
        {name:'1号车'},
        {name:'4号车'},
        {name:'2号车'},
        {name:'1号车'},
        {name:'2号车'},
         {name:'4号车'},
        {name:'1号车'},
        {name:'4号车'},
      ],
      time8:[
       {time:'时间'},
        {time:'10:30'},
        {time:'15:15'},
        {time:'16:35'}
      ],
       car8:[
         {name:'车辆'},
        {name:'4号车'},
        {name:'4号车'},
        {name:'4号车'}
      ]
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
#bbox table{
  border:1px black solid;
}
#bbox table td{
  width:125px;
  padding-bottom:6px;
}
#bbox table td:first-child{color:#2eaced;font-size: 1.2em;}
#note table td:first-child{color:black;}
#note{
  float:right;
text-align: left;
width: 450px;
background-color: #d9f7f2;
padding:8px 8px;
margin-left:25px;
margin-top: 20px;
}
#position{
  margin-top:50px;
}
#position table td{
  border: 1px grey solid;
}
#position table{
   border-collapse: collapse;
}


</style>