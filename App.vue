<template>
  <List :data="data"/>
</template>

<script>
import List from './List'

export default {
  data () {
    return {
      data: [
        {
          title: '体育明星',
          children: [
            {
              title: '游泳',
              children: [
                {
                  title: '孙杨'
                },
                {
                  title: '傅园慧'
                }
              ]
            }
          ]
        },
        {
          title: '篮球',
          children: [
            {
              title: 'NBA',
              children: [
                {
                  title: '勇士',
                  children: [
                    {
                      title: '库里',
                      children: [
                        {
                          title: 'MVP'
                        },
                        {
                          title: '得分王'
                        }
                      ]
                    },
                    {
                      title: '汤普森'
                    }
                  ]
                },
                {
                  title: '火箭',
                  children: [
                    {
                      title: '哈登'
                    },
                    {
                      title: '维斯布鲁克'
                    }
                  ]
                }
              ]
            }
          ]
        }
      ]
    }
  },
  components: {
    List
  }
}
</script>

<style>

</style>
