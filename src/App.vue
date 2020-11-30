<template>
    
  <div id="app">
    <div id="cal">
    <el-select v-model="value1" placeholder="请选择数字" style="margin-right:15px;">
    <el-option
      v-for="item in options"
      :key="item.value"
      :label="item.label"
      :value="item.value">
    </el-option>
  </el-select>
  <el-select v-model="operator" placeholder="请选择符号" style="margin-right:15px;">
    <el-option
      v-for="operators in operators"
      :key="operators.value"
      :label="operators.label"
      :value="operators.value">
    </el-option>
  </el-select>
  <el-select v-model="value2" placeholder="请选择数字" style="margin-right:15px;">
    <el-option
      v-for="item2 in 100"
      :key="item2"
      :label="item2"
      :value="item2">
    </el-option>
  </el-select>
  <!-- <el-select v-model="value3" placeholder="请选择数字" style="margin-right:15px;">
    <el-option
      v-for="item2 in 100"
      :key="item2"
      :label="item2"
      :value="item2">
    </el-option>
  </el-select> -->
  <span> </span>
  <el-button type="primary" @click="cal(value1,operator,value2)">执行</el-button>
  </div>
  </br>
  </br>

  <div id="test">
    <font size="66px" color="grey">执行结果:</font>
  <font size="88px">{{result}}</font>
  </div>
  
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'app',
  components: {
    HelloWorld
  },
  methods:{
    cal:function(value1,operator,value2){

      if(operator=='+'){
        console.log('test');
        this.result=value1+value2;
      }

      if(operator=='-')
      this.result=value1-value2;
      if(operator=='*')
      this.result=value1*value2;
      if(operator=='/')
      this.result=value1/value2;
        console.log(value1);

    }
  },
  data() {
      return {
        options: [{
          // value: 'value1-2',
          value: 2,
          label: 2
        }, {
          value: 4,
          label: 4
        }, {
          value: 8,
          label: 8
        }, {
          value: 16,
          label: 16
        }, {
          value: 32,
          label: 32
        },{
          value: 64,
          label: 64
        },{
          value: 128,
          label: 128
        },{
          value: 256,
          label: 256
        },{
          value: 512,
          label: 512
        },{
          value: 1024,
          label: 1024
        }
        ],
        
        value1: '',
        operator:'',
        value2:'',
        value3:'',
        operators:[{
          value: '+',
          label: '+'
        },{
          value: '-',
          label: '-'
        },{
          value: '*',
          label: '*'
        },{
          value: '/',
          label: '/'
        },],
        options2:[{
          // value: 'value2-1',
          value: 1,
          label: 1
        },
        {
          value: 2,
          label: 2
        },{
          value: 3,
          label: 3
        },{
          value: 4,
          label: 4
        },{
          value: 5,
          label: 5
        },{
          value: 6,
          label: 6
        },{
          value: 'value2-7',
          label: 7
        },{
          value: 'value2-8',
          label: 8
        },{
          value: 'value2-9',
          label: 9
        },{
          value: 'value2-10',
          label: 10
        },{
          value: 'value2-11',
          label: 11
        },{
          value: 'value2-12',
          label: 12
        },{
          value: 'value2-13',
          label: 13
        },{
          value: 'value2-14',
          label: 14
        },{
          value: 'value2-15',
          label: 15
        },{
          value: 'value2-16',
          label: 16
        },{
          value: 'value2-17',
          label: 17
        },{
          value: 'value2-18',
          label: 18
        },{
          value: 'value2-19',
          label: 19
        },{
          value: 'value2-20',
          label: 20
        },{
          value: 'value2-21',
          label: 21
        },{
          value: 'value2-22',
          label: 22
        },{
          value: 'value2-23',
          label: 23
        },{
          value: 'value2-24',
          label: 24
        },{
          value: 'value2-25',
          label: 25
        },{
          value: 'value2-26',
          label: 26
        },{
          value: 'value2-27',
          label: 27
        },{
          value: 'value2-28',
          label: 28
        },{
          value: 'value2-29',
          label: 29
        },{
          value: 'value2-30',
          label: 30
        },{
          value: 'value2-31',
          label: 31
        },{
          value: 'value2-32',
          label: 32
        },{
          value: 'value2-33',
          label: 33
        },{
          value: 'value2-34',
          label: 34
        },{
          value: 'value2-35',
          label: 35
        },{
          value: 'value2-36',
          label: 36
        },{
          value: 'value2-37',
          label: 37
        },{
          value: 'value2-38',
          label: 38
        },{
          value: 'value2-39',
          label: 39
        },{
          value: 'value2-40',
          label: 40
        },{
          value: 'value2-41',
          label: 41
        },{
          value: 'value2-42',
          label: 42
        },{
          value: 'value2-43',
          label: 43
        },{
          value: 'value2-44',
          label: 44
        },{
          value: 'value2-45',
          label: 45
        },{
          value: 'value2-46',
          label: 46
        },{
          value: 'value2-47',
          label: 47
        },{
          value: 'value2-48',
          label: 48
        },{
          value: 'value2-49',
          label: 49
        },{
          value: 'value2-50',
          label: 50
        },{
          value: 'value2-51',
          label: 51
        },{
          value: 'value2-52',
          label: 52
        },{
          value: 'value2-53',
          label: 53
        },{
          value: 'value2-54',
          label: 54
        },{
          value: 'value2-55',
          label: 55
        },{
          value: 'value2-56',
          label: 56
        },{
          value: 'value2-57',
          label: 57
        },{
          value: 'value2-58',
          label: 58
        },{
          value: 'value2-59',
          label: 59
        },{
          value: 'value2-60',
          label: 60
        },{
          value: 'value2-61',
          label: 61
        },{
          value: 'value2-62',
          label: 62
        },{
          value: 'value2-63',
          label: 63
        },{
          value: 'value2-64',
          label: 64
        },{
          value: 'value2-65',
          label: 65
        },{
          value: 'value2-66',
          label: 66
        },{
          value: 'value2-67',
          label: 67
        },{
          value: 'value2-68',
          label: 68
        },{
          value: 'value2-69',
          label: 69
        },{
          value: 'value2-70',
          label: 70
        },{
          value: 'value2-71',
          label: 71
        },{
          value: 'value2-72',
          label: 72
        },{
          value: 'value2-73',
          label: 73
        },{
          value: 'value2-74',
          label: 74
        },{
          value: 'value2-75',
          label: 75
        },{
          value: 'value2-76',
          label: 76
        },{
          value: 'value2-77',
          label: 77
        },{
          value: 'value2-78',
          label: 78
        },{
          value: 'value2-79',
          label: 79
        },{
          value: 'value2-80',
          label: 80
        },{
          value: 'value2-81',
          label: 81
        },{
          value: 'value2-82',
          label: 82
        },{
          value: 'value2-83',
          label: 83
        },{
          value: 'value2-84',
          label: 84
        },{
          value: 'value2-85',
          label: 85
        },{
          value: 'value2-86',
          label: 86
        },{
          value: 'value2-87',
          label: 87
        },{
          value: 'value2-88',
          label: 88
        },{
          value: 'value2-89',
          label: 89
        },{
          value: 'value2-90',
          label: 90
        },{
          value: 'value2-91',
          label: 91
        },{
          value: 'value2-92',
          label: 92
        },{
          value: 'value2-93',
          label: 93
        },{
          value: 'value2-94',
          label: 94
        },{
          value: 'value2-95',
          label: 95
        },{
          value: 'value2-96',
          label: 96
        },{
          value: 'value2-97',
          label: 97
        },{
          value: 'value2-98',
          label: 98
        },{
          value: 'value2-99',
          label: 99
        },{
          value: 'value2-100',
          label: 100
        },
        ],
        result:'',
      }
    }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  box-shadow: gray;
  margin:5px;
}
#test{
  background-color:transparent;
  box-shadow: 2px 2px grey;
}
#cal{
    background-color:transparent;
  box-shadow: 2px 2px grey;
}
</style>
