<template>
  <div id="ranking-board">
    <div class="ranking-board-title">生产数量排名</div>
    <dv-scroll-ranking-board :config="config" />
  </div>
</template>

<script>
export default {
  name: 'RankingBoard',
  data () {
    return {
      config: {
        data: [
          {
            name: '基地1',
            value: 55
          },
          {
            name: '基地2',
            value: 120
          },
          {
            name: '基地3',
            value: 78
          },
          {
            name: '基地4',
            value: 66
          },
          {
            name: '基地5',
            value: 80
          },
          {
            name: '基地6',
            value: 45
          },
          {
            name: '基地7',
            value: 29
          },
          {
            name: '基地8',
            value: 29
          },
          {
            name: '基地9',
            value: 29
          }
        ],
        rowNum: 9
      }
    }
  }
}
</script>

<style lang="less">
#ranking-board {
  width: 20%;
  box-shadow: 0 0 3px blue;
  display: flex;
  flex-direction: column;
  background-color: rgba(6, 30, 93, 0.5);
  border-top: 2px solid rgba(1, 153, 209, .5);
  box-sizing: border-box;
  padding: 0px 30px;

  .ranking-board-title {
    font-weight: bold;
    height: 50px;
    display: flex;
    align-items: center;
    font-size: 20px;
  }

  .dv-scroll-ranking-board {
    flex: 1;
  }
}
</style>
