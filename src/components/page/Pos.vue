<template>
    <div class="pos">
        <el-row>
            <el-col :span="7" class="pos-order" id="order-list">
                <el-tabs>
                    <el-tab-pane label="点餐">
                        <el-table :data="tableData" border>
                            <el-table-column prop="goodsName" label="商品名称">
                                
                            </el-table-column>
                            <el-table-column prop="count" label="数量" width="70">

                            </el-table-column>
                            <el-table-column prop="price" label="金额" width="70">

                            </el-table-column>
                            <el-table-column prop="actions" label="操作" width="100" fixed="right">
                                <template>
                                    <el-button type="text" size="small">删除</el-button>
                                    <el-button type="text" size="small">添加</el-button>
                                </template>
                            </el-table-column>
                        </el-table>
												<div>
													<el-button type="warning">挂单s123</el-button>
													<el-button type="">删除</el-button>
													<el-button type="">结账</el-button>
												</div>
                    </el-tab-pane>
                    <el-tab-pane label="挂单">
                        挂单
                    </el-tab-pane>
                    <el-tab-pane label="外卖">
                        外卖
                    </el-tab-pane>
                </el-tabs>
            </el-col>
            <el-col :span="7" class="pos-product">
                我是产品
            </el-col>
        </el-row>
    </div>
</template>

<script>
export default {
  name: 'pos',
  data(){
    return {
      tableData: [{
          goodsName: '可口可乐',
          price: 8,
          count:1
        }, {
          goodsName: '香辣鸡腿堡',
          price: 15,
          count:1
        }, {
          goodsName: '爱心薯条',
          price: 8,
          count:1
        }, {
          goodsName: '甜筒',
          price: 8,
          count:1
				}
			]
    }
  },
  // 所有的虚拟DOM加载完成之后执行
  mounted: function(){
    var orderHeight = document.documentElement.clientHeight
    document.getElementById('order-list').style.height = orderHeight + 'px'
  }
}
</script>

<style scoped lang="less">
.pos {
  height: 100%;
  .pos-order {
    border-right: 1px solid #ccc;
    background-color: #eee;
    text-align: center;
    .el-tabs__item {
        text-align: center;
    }
  }
  .pos-product {
    background-color: #ddd;
  }
}
</style>

