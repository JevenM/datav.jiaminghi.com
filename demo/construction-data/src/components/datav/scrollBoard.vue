<template>
  <div id="scroll-board">
    <dv-scroll-board :config="config" />
  </div>
</template>

<script>
export default {
  name: 'ScrollBoard',
  data () {
    return {
      config: {
        header: ['时间', '危险信息', '数量', '地址'],
        data: [
          ['2019-07-01 19:25:00', '人为破坏', '5', 'xxxxxxx'],
          ['2019-07-02 17:25:00', '虫灾', '13', 'xxxxxxx'],
          ['2019-07-03 16:25:00', '雨水灾害', '6', 'xxxxxxx'],
          ['2019-07-04 15:25:00', '高温预警', '2', 'xxxxxxx'],
          ['2019-07-05 14:25:00', '低温预警', '1', 'xxxxxxx'],
          ['2019-07-06 13:25:00', '紫外线过强', '3', 'xxxxxxx'],
          ['2019-07-07 12:25:00', '其他自然灾害1', '4', 'xxxxxxx'],
          ['2019-07-08 11:25:00', '其他自然灾害2', '2', 'xxxxxxx'],
          ['2019-07-09 10:25:00', '其他自然灾害3', '5', 'xxxxxxx'],
          ['2019-07-10 09:25:00', '其他自然灾害4', '3', 'xxxxxxx']
        ],
        index: true,
        columnWidth: [50, 170, 300],
        align: ['center'],
        rowNum: 7,
        headerBGC: '#1981f6',
        headerHeight: 45,
        oddRowBGC: 'rgba(0, 44, 81, 0.8)',
        evenRowBGC: 'rgba(10, 29, 50, 0.8)'
      }
    }
  }
}
</script>

<style lang="less">
#scroll-board {
  width: 50%;
  box-sizing: border-box;
  margin-left: 20px;
  height: 100%;
  overflow: hidden;
}
</style>
