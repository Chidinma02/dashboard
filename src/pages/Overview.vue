<template>
  <div class="content">
    <div class="container-fluid">
      <p>Welcome back,Anthony</p>
      <p>Dashboard</p>
      <div class="row">
       
        <div class="col-xl-3 col-md-6 ml-0 pl-0">
          <stats-card>
            <div slot="header" class="icon-warning">
              <p class="card-category">Total Products</p>
              <h4 class="card-title">30,000</h4>
             
            </div>
            <div slot="content">
              <img src="../../public/img/Frame 1171276850.png" class="dr">
              
            </div>
            <!-- <div slot="footer">
              <i class="fa fa-refresh"></i>Updated now
            </div> -->
          </stats-card>
        </div>

        <div class="col-xl-3 col-md-6 ml-0 pl-0">
          <stats-card>
            <div slot="header" class="icon-warning">
              <p class="card-category">Total Products</p>
              <h4 class="card-title">30,000</h4>
             
            </div>
            <div slot="content">
              <img src="../../public/img/Frame 1171276850 (1).png" class="dr">
            </div>
            <!-- <div slot="footer">
              <i class="fa fa-refresh"></i>Updated now
            </div> -->
          </stats-card>
        </div>

        <div class="col-xl-3 col-md-6 ml-0 pl-0">
          <stats-card>
            <div slot="header" class="icon-warning">
              <p class="card-category">Total Products</p>
              <h4 class="card-title">30,000</h4>
             
            </div>
            <div slot="content">
              <img src="../../public/img/Frame 1171276850 (2).png" class="dr">
            </div>
            <!-- <div slot="footer">
              <i class="fa fa-refresh"></i>Updated now
            </div> -->
          </stats-card>
        </div>
        <div class="col-xl-3 col-md-6 ml-0 pl-0">
          <stats-card>
            <div slot="header" class="icon-warning">
              <p class="card-category">Total Products</p>
              <h4 class="card-title">30,000</h4>
             
            </div>
            <div slot="content">
              <img src="../../public/img/Frame 1171276850 (2).png" class="dr">
               
            </div>
            <!-- <div slot="footer">
              <i class="fa fa-refresh"></i>Updated now
            </div> -->
          </stats-card>
        </div>

      </div>
      <div class="row">
        <div class="col-md-8">
          <chart-card :chart-data="lineChart.data"
                      :chart-options="lineChart.options"
                      :responsive-options="lineChart.responsiveOptions">
            <template slot="header">
              <h4 class="card-title">General Sales Activity</h4>
              
            </template>
          
          </chart-card>
        </div>

        <div class="col-md-4">
          <!-- <chart-card :chart-data="pieChart.data" chart-type="Pie"> -->
            
              <p class="card-title">New messages</p>
              <h1 class="">2</h1>
              <p><a href="">View messages</a></p>
        
            <!-- <template slot="footer">
              <div class="legend">
                <i class="fa fa-circle text-info"></i> Open
                <i class="fa fa-circle text-danger"></i> Bounce
                <i class="fa fa-circle text-warning"></i> Unsubscribe
              </div>
              <hr>
              <div class="stats">
                <i class="fa fa-clock-o"></i> Campaign sent 2 days ago
              </div>
            </template> -->
          <!-- </chart-card> -->
        </div>
      </div>
     

      <div class="row">
        <div class="col-lg-12 df">
          <h6>New Order</h6>
          <!-- <chart-card
            :chart-data="barChart.data"
            :chart-options="barChart.options"
            :chart-responsive-options="barChart.responsiveOptions"
            chart-type="Bar">
            <template slot="header">
              <h4 class="card-title">2014 Sales</h4>
              <p class="card-category">All products including Taxes</p>
            </template>
            <template slot="footer">
              <div class="legend">
                <i class="fa fa-circle text-info"></i> Tesla Model S
                <i class="fa fa-circle text-danger"></i> BMW 5 Series
              </div>
              <hr>
              <div class="stats">
                <i class="fa fa-check"></i> Data information certified
              </div>
            </template>
          </chart-card> -->

          <table class="table table-borderless text-nowrap ">
  <thead>
    <tr>
      <th scope="col">Time</th>
      <th scope="col">Name</th>
      <th scope="col">Email</th>
      <th scope="col-2">Phone</th>
      <th scope="col-2">Location</th>
      <th scope="col">Items</th>
      <th scope="col">Price</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">8:00</th>
      
      <td>David mark</td>
      <td>@mdo</td>
      <td>080123456789</td>
      <td>10,yemi ogunleye</td>
      <td>2px paracetamol injection</td>
      <td>3,000</td>
    </tr>
    <tr>
      <th scope="row">8:00</th>
      
      <td>David mark</td>
      <td>@mdo</td>
      <td>080123456789</td>
      <td>10,yemi ogunleye</td>
      <td>2px paracetamol injection</td>
      <td>3,000</td>
    </tr>
    <tr>
      <th scope="row">8:00</th>
    
      <td>David mark</td>
      <td>@mdo</td>
      <td>080123456789</td>
      <td>10,yemi ogunleye</td>
      <td>2px paracetamol injection</td>
      <td>3,000</td>
    </tr>
    
  </tbody>
</table>
        </div>

        <!-- <div class="col-md-6">
          <card>
            <template slot="header">
              <h5 class="title">Tasks</h5>
              <p class="category">Backend development</p>
            </template>
            <l-table :data="tableData.data"
                     :columns="tableData.columns">
              <template slot="columns"></template>

              <template slot-scope="{row}">
                <td>
                  <base-checkbox v-model="row.checked"></base-checkbox>
                </td>
                <td>{{row.title}}</td>
                <td class="td-actions text-right">
                  <button type="button" class="btn-simple btn btn-xs btn-info" v-tooltip.top-center="editTooltip">
                    <i class="fa fa-edit"></i>
                  </button>
                  <button type="button" class="btn-simple btn btn-xs btn-danger" v-tooltip.top-center="deleteTooltip">
                    <i class="fa fa-times"></i>
                  </button>
                </td>
              </template>
            </l-table>
            <div class="footer">
              <hr>
              <div class="stats">
                <i class="fa fa-history"></i> Updated 3 minutes ago
              </div>
            </div>
          </card>

        </div> -->
      </div>
    </div>
  </div>
</template>
<script>
  import ChartCard from 'src/components/Cards/ChartCard.vue'
  import StatsCard from 'src/components/Cards/StatsCard.vue'
  import LTable from 'src/components/Table.vue'

  export default {
    components: {
      LTable,
      ChartCard,
      StatsCard
    },
    data () {
      return {
        editTooltip: 'Edit Task',
        deleteTooltip: 'Remove',
        pieChart: {
          data: {
            labels: ['40%', '20%', '40%'],
            series: [40, 20, 40]
          }
        },
        lineChart: {
          data: {
            labels: ['9:00AM', '12:00AM', '3:00PM', '6:00PM', '9:00PM', '12:00PM', '3:00AM', '6:00AM'],
            series: [
              [287, 385, 490, 492, 554, 586, 698, 695],
              [67, 152, 143, 240, 287, 335, 435, 437],
              [23, 113, 67, 108, 190, 239, 307, 308]
            ]
          },
          options: {
            low: 0,
            high: 800,
            showArea: false,
            height: '245px',
            axisX: {
              showGrid: false
            },
            lineSmooth: true,
            showLine: true,
            showPoint: true,
            fullWidth: true,
            chartPadding: {
              right: 50
            }
          },
          responsiveOptions: [
            ['screen and (max-width: 640px)', {
              axisX: {
                labelInterpolationFnc (value) {
                  return value[0]
                }
              }
            }]
          ]
        },
        barChart: {
          data: {
            labels: ['Jan', 'Feb', 'Mar', 'Apr', 'Mai', 'Jun', 'Jul', 'Aug', 'Sep', 'Oct', 'Nov', 'Dec'],
            series: [
              [542, 443, 320, 780, 553, 453, 326, 434, 568, 610, 756, 895],
              [412, 243, 280, 580, 453, 353, 300, 364, 368, 410, 636, 695]
            ]
          },
          options: {
            seriesBarDistance: 10,
            axisX: {
              showGrid: false
            },
            height: '245px'
          },
          responsiveOptions: [
            ['screen and (max-width: 640px)', {
              seriesBarDistance: 5,
              axisX: {
                labelInterpolationFnc (value) {
                  return value[0]
                }
              }
            }]
          ]
        },
        tableData: {
          data: [
            {title: 'Sign contract for "What are conference organizers afraid of?"', checked: false},
            {title: 'Lines From Great Russian Literature? Or E-mails From My Boss?', checked: true},
            {
              title: 'Flooded: One year later, assessing what was lost and what was found when a ravaging rain swept through metro Detroit',
              checked: true
            },
            {title: 'Create 4 Invisible User Experiences you Never Knew About', checked: false},
            {title: 'Read "Following makes Medium better"', checked: false},
            {title: 'Unfollow 5 enemies from twitter', checked: false}
          ]
        }
      }
    }
  }
</script>
<style>
.card-category{
  font-size:10px !important;
}

.card-title{
  font-size:20px !important;
}
.card{
  border:1px solid rgb(223, 223, 223)!important
}
.dr{
  width:40px;
  height:40px;
}
.df{
  font:10px !important;
}
</style>
