<template>
  <div>

    <nut-searchbar placeText="请输入自定义文案"></nut-searchbar>

    <nut-row type="flex"
             flexWrap="wrap"
             :gutter="10"
             ustify="center">
      <nut-col :span="5">
        <!-- <div class="flex-content">1</div> -->
        <nut-button type="primary"
                    shape="circle"
                    small
                    color="rgb(0,0,0)" />
      </nut-col>
      <nut-col :span="5">
        <div class="flex-content flex-content-light">2</div>
      </nut-col>

      <nut-col :span="5">
        <div class="flex-content">3</div>
      </nut-col>
      <nut-col :span="5">
        <div class="flex-content flex-content-light">4</div>
      </nut-col>

      <nut-col :span="5">
        <div class="flex-content">5</div>
      </nut-col>

      <!-- </nut-row>

    <nut-row type="flex"
             flexWrap="wrap"
             :gutter="10"
             ustify="center"> -->

      <nut-col :span="5">
        <div class="flex-content flex-content-light">2</div>
      </nut-col>
    </nut-row>
    <nut-tabbar @tab-switch="tabSwitch3"
                :tabbarList="tabList3"
                :bottom="true">
    </nut-tabbar>

  </div>

</template>




<script>
export default {

  data () {
    return {
      tabList3: [
        {
          'tabTitle': '首页',
          'curr': true,
          'icon': 'http://img13.360buyimg.com/uba/jfs/t1/29316/38/1115/3203/5c0f3d61E35d0c7da/9e557f2cb5c9dab6.jpg',
          'activeIcon': 'http://img20.360buyimg.com/uba/jfs/t1/9996/36/8646/4833/5c0f3d61E7c1b7e0f/c98ad61124172e93.jpg',
          'href': '###'
        },
        {
          'tabTitle': '分类',
          'curr': false,
          'icon': 'http://img12.360buyimg.com/uba/jfs/t1/25443/23/1062/4600/5c0f3d61E2e9f1360/c9b3421fe18614e2.jpg',
          'activeIcon': 'http://img20.360buyimg.com/uba/jfs/t1/19241/12/1048/8309/5c0f3d61E17ed5a56/c3af0964cade47f8.jpg',
          'href': '###'
        },
        {
          'tabTitle': '发现',
          'curr': false,
          'icon': 'http://img13.360buyimg.com/uba/jfs/t1/10361/35/4713/4643/5c0f3d62E437a3c94/273fd0fb90798f03.jpg',
          'activeIcon': 'http://img14.360buyimg.com/uba/jfs/t1/26604/35/1073/7896/5c0f3d61Eb9f5f184/5f01c938abe4216d.jpg',
          'href': '###'
        },
        {
          'tabTitle': '购物车',
          'curr': false,
          'num': 2,
          'icon': 'http://img11.360buyimg.com/uba/jfs/t1/14848/18/1066/3723/5c0f41bdE9f2a38fe/e6ed6768717297fb.jpg',
          'activeIcon': 'http://img30.360buyimg.com/uba/jfs/t1/17538/16/1070/6214/5c0f41bdE4bc9a1db/74cf978e5015454b.jpg',
          'href': '###'
        },
        {
          'tabTitle': '我的',
          'curr': false,
          'icon': 'http://img20.360buyimg.com/uba/jfs/t1/20004/20/1045/3620/5c0f3d61Eaaec1670/9e59db63983b7b9f.jpg',
          'activeIcon': 'http://img14.360buyimg.com/uba/jfs/t1/23967/14/1072/6714/5c0f3d61E0ad8991e/8f741953f6e38f15.jpg',
          'href': '###'
        }
      ]
    };
  },
  methods: {
    tabSwitch3: function (value, index) {
      console.log(index);
    }
  }
};
</script>