<template>
  <div class="content"  >
    <div class="container-fluid">
      <h5 class="bt  ">Welcome Back, Anthony</h5>
        <h5 class="mt-3 bt">All Orders</h5>

        <nav>
  <div class="nav nav-tabs" id="nav-tab" role="tablist">
    <button class="nav-link active" id="nav-home-tab" data-bs-toggle="tab" data-bs-target="#nav-home" type="button" role="tab" aria-controls="nav-home" aria-selected="true">Home</button>
    <button class="nav-link" id="nav-profile-tab" data-bs-toggle="tab" data-bs-target="#nav-profile" type="button" role="tab" aria-controls="nav-profile" aria-selected="false">Profile</button>
    <button class="nav-link" id="nav-contact-tab" data-bs-toggle="tab" data-bs-target="#nav-contact" type="button" role="tab" aria-controls="nav-contact" aria-selected="false">Contact</button>
  </div>
</nav>
<div class="tab-content" id="nav-tabContent">
  <div class="tab-pane fade show active" id="nav-home" role="tabpanel" aria-labelledby="nav-home-tab">...</div>
  <div class="tab-pane fade" id="nav-profile" role="tabpanel" aria-labelledby="nav-profile-tab">...</div>
  <div class="tab-pane fade" id="nav-contact" role="tabpanel" aria-labelledby="nav-contact-tab">...</div>
</div>
<div class="tab-content" id="myTabContent">
  <div class="tab-pane fade show active" id="home" role="tabpanel" aria-labelledby="home-tab">chidddd</div>
  <div class="tab-pane fade" id="profile" role="tabpanel" aria-labelledby="profile-tab">dddddddddddd</div>
  <div class="tab-pane fade" id="contact" role="tabpanel" aria-labelledby="contact-tab">eeeeeeeeeeee</div>
</div>
      <div class="row hu">
        
      

        <div class="col-12">
         

<table class="table table-borderless text-nowrap  tab">
  <thead>
    <tr>
      <th scope="col tab" style="color:#258576;" >Time</th>
      <th scope="col tab" style="color:#258576;">Full Name</th>
      <th scope="col tab" style="color:#258576;">Email</th>
      <th scope="col tab" style="color:#258576;">Phone</th>
      <th scope="col tab" style="color:#258576;">Location</th>
      <th scope="col tab" style="color:#258576;">prescription</th>
      <th scope="col tab" style="color:#258576;">Price</th>
    </tr>
  </thead>
  <tbody class="cont">
    <tr>
      <th scope="row">8:00</th>
      
      <td class="tab">David mark</td>
      <td>@mdo</td>
      <td>080123456789</td>
      <td>Ikeja,Lagos</td>
      <td>2px paracetamol injection</td>
      <td>3,000</td>
    </tr>
    <tr>
      <th scope="row">8:00</th>
      
      <td>David mark</td>
      <td>@mdo</td>
      <td>080123456789</td>
      <td>Ikeja,Lagos</td>
      <td>2px paracetamol injection</td>
      <td>3,000</td>
    </tr>
    <tr>
      <th scope="row">8:00</th>
    
      <td>David mark</td>
      <td>@mdo</td>
      <td>080123456789</td>
      <td>Ikeja,Lagos</td>
      <td>2px paracetamol injection</td>
      <td>3,000</td>
    </tr>
    
  </tbody>
</table>
        </div>
        <table>
  <tr>
    <td class="red-text yellow-background">This is a red text on a yellow background.</td>
  </tr>
</table>
<table>
  <tr>
    <th style="color: red; background-color: yellow;">Header 1</th>
    <th style="color: blue; background-color: green;">Header 2</th>
  </tr>
</table>

        <!-- <div class="col-12">
          <card class="strpied-tabled-with-hover"
                body-classes="table-full-width table-responsive"
          >
            <template slot="header">
              <h4 class="card-title">Small table</h4>
              <p class="card-category">Here is a subtitle for this table</p>
            </template>
            <l-table class="table-hover table-striped table-sm"
                     :columns="table1.columns"
                     :data="table1.data">
            </l-table>
          </card>

        </div> -->

      </div>
    </div>
  </div>
</template>
<script>
  import LTable from 'src/components/Table.vue'
  import Card from 'src/components/Cards/Card.vue'
  const tableColumns = ['Id', 'FullName', 'emailaddress', 'Country', 'City']
  const tableData = [{
    id: 1,
    FullName: 'Dakota Rice',
    emailaddress: '$36.738',
    country: 'Niger',
    city: 'Oud-Turnhout'
  },
  {
    id: 2,
    FullName: 'Minerva Hooper',
    emailaddress: '$23,789',
    country: 'Curaçao',
    city: 'Sinaai-Waas'
  },
  {
    id: 3,
    FullName: 'Sage Rodriguez',
    emailaddress: '$56,142',
    country: 'Netherlands',
    city: 'Baileux'
  },
  {
    id: 4,
    FullName: 'Philip Chaney',
    emailaddress: '$38,735',
    country: 'Korea, South',
    city: 'Overland Park'
  },
  {
    id: 5,
    FullName: 'Doris Greene',
    emailaddress: '$63,542',
    country: 'Malawi',
    city: 'Feldkirchen in Kärnten'
  }]
  export default {
    components: {
      LTable,
      Card
    },
    data () {
      return {
        table1: {
          columns: [...tableColumns],
          data: [...tableData]
        },
        table2: {
          columns: [...tableColumns],
          data: [...tableData]
        }
      }
    }
  }
</script>
<style>
.hu{
  background-color:whitesmoke;
  
}
.bt{
  font-weight:550;
}
.tab{
  color: red !important;

}
.red-text {
  color: red;
}
.yellow-background {
  background-color: yellow;
}
.cont{
  color:red !important;
}
</style>
