<template>
  
  <div class="cc">

    <div class="row mb-3 ">
    
      <div class="col-10">
       
      <h5>Welcome Back,Anthony</h5>
        <!-- <button class="bt-new">New product</button>  -->
      </div>
      <div class="col-2">
        <!-- <button type="button" class="btn btn-outline-light">Light</button> -->
        <button class="bt-new btn">New product</button> 
      </div>
    </div>
   
     <div class="row ">
      <div class="col-md-4" v-for="post in this.posts " :key="post.id">
        <div>
          <!-- <img :src="post.image"  class="img-fluid"> -->
          <img src="../../../public/img/Frame 83.png"  class="img-fluid">
          <div class="row ">
            <div class="col-8">
              <p class="ge">{{post.drug_name
 }}</p>
            
              <!-- <p class="fr fe">Anti retroviral</p> -->
              <p class="fr fe">{{ post. composition}}</p>
              <p class="fr fe"><img src="../../../public/img/Ellipse 43.png" class="img-fluid lu"> Available</p>
              <p class="fr fe"><img src="../../../public/img/Ellipse 43.png" class="img-fluid lu"> In stock</p>
            </div>
            <div class="col-4">
              <p class="ge">{{ post.presentation }}</p>
              
            </div>
          </div>
         

        </div>
      </div>
      <!-- <div class="col-md-4">
        <div>
          <img src="../../../public/img/Frame 83.png" class="img-fluid">
          <div class="row ">
            <div class="col-8">
              <p class="ge">Lamivudine 150mg</p>
            
              <p class="fr fe">Anti retroviral</p>
              <p class="fr fe"><img src="../../../public/img/Ellipse 43.png" class="img-fluid lu"> Available</p>
              <p class="fr fe"><img src="../../../public/img/Ellipse 43.png" class="img-fluid lu"> In stock</p>
            </div>
            <div class="col-4">
              <p class="ge">N 2,800</p>
              
            </div>
          </div>
         

        </div>
      </div> -->
      <!-- <div class="col-md-4">
        <div>
          <img src="../../../public/img/Frame 83.png" class="img-fluid">
          <div class="row ">
            <div class="col-8">
              <p class="ge">Lamivudine 150mg</p>
            
              <p class="fr fe">Anti retroviral</p>
              <p class="fr fe"><img src="../../../public/img/Ellipse 43.png" class="img-fluid lu"> Available</p>
              <p class="fr fe"><img src="../../../public/img/Ellipse 43.png" class="img-fluid lu"> In stock</p>
            </div>
            <div class="col-4">
              <p class="ge">N 2,800</p>
              
            </div>
          </div>
         

        </div>
      </div> -->
     </div> 
      <!-- <div class="row mt-5">
      <div class="col-md-4">
        <div>
          <img src="../../../public/img/Frame 83.png" class="img-fluid">
          <div class="row ">
            <div class="col-8">
              <p class="ge">Lamivudine 150mg</p>
            
              <p class="fr fe">Anti retroviral</p>
              <p class="fr fe"><img src="../../../public/img/Ellipse 43.png" class="img-fluid lu"> Available</p>
              <p class="fr fe"><img src="../../../public/img/Ellipse 43.png" class="img-fluid lu"> In stock</p>
            </div>
            <div class="col-4">
              <p class="ge">N 2,800</p>
              
            </div>
          </div>
         

        </div>
      </div>
      <div class="col-md-4">
        <div>
          <img src="../../../public/img/Frame 83.png" class="img-fluid">
          <div class="row ">
            <div class="col-8">
              <p class="ge">Lamivudine 150mg</p>
            
              <p class="fr fe">Anti retroviral</p>
              <p class="fr fe"><img src="../../../public/img/Ellipse 43.png" class="img-fluid lu"> Available</p>
              <p class="fr fe"><img src="../../../public/img/Ellipse 43.png" class="img-fluid lu"> In stock</p>
            </div>
            <div class="col-4">
              <p class="ge">N 2,800</p>
              
            </div>
          </div>
         

        </div>
      </div>
      <div class="col-md-4">
        <div>
          <img src="../../../public/img/Frame 83.png" class="img-fluid">
          <div class="row ">
            <div class="col-8">
              <p class="ge">Lamivudine 150mg</p>
            
              <p class="fr fe">Anti retroviral</p>
              <p class="fr fe"><img src="../../../public/img/Ellipse 43.png" class="img-fluid lu"> Available</p>
              <p class="fr fe"><img src="../../../public/img/Ellipse 43.png" class="img-fluid lu"> In stock</p>
            </div>
            <div class="col-4">
              <p class="ge">N 2,800</p>
              
            </div>
          </div>
         

        </div>
      </div>
     </div>
     <div class="row mt-5">
      <div class="col-md-4">
        <div>
          <img src="../../../public/img/Frame 83.png" class="img-fluid">
          <div class="row ">
            <div class="col-8">
              <p class="ge">Lamivudine 150mg</p>
            
              <p class="fr fe">Anti retroviral</p>
              <p class="fr fe"><img src="../../../public/img/Ellipse 43.png" class="img-fluid lu"> Available</p>
              <p class="fr fe"><img src="../../../public/img/Ellipse 43.png" class="img-fluid lu"> In stock</p>
            </div>
            <div class="col-4">
              <p class="ge">N 2,800</p>
              
            </div>
          </div>
         

        </div>
      </div>
      <div class="col-md-4">
        <div>
          <img src="../../../public/img/Frame 83.png" class="img-fluid">
          <div class="row ">
            <div class="col-8">
              <p class="ge">Lamivudine 150mg</p>
            
              <p class="fr fe">Anti retroviral</p>
              <p class="fr fe"><img src="../../../public/img/Ellipse 43.png" class="img-fluid lu"> Available</p>
              <p class="fr fe"><img src="../../../public/img/Ellipse 43.png" class="img-fluid lu"> In stock</p>
            </div>
            <div class="col-4">
              <p class="ge">N 2,800</p>
              
            </div>
          </div>
         

        </div>
      </div>
      <div class="col-md-4">
        <div>
          <img src="../../../public/img/Frame 83.png" class="img-fluid">
          <div class="row ">
            <div class="col-8">
              <p class="ge">Lamivudine 150mg</p>
            
              <p class="fr fe">Anti retroviral</p>
              <p class="fr fe"><img src="../../../public/img/Ellipse 43.png" class="img-fluid lu"> Available</p>
              <p class="fr fe"><img src="../../../public/img/Ellipse 43.png" class="img-fluid lu"> In stock</p>
            </div>
            <div class="col-4">
              <p class="ge">N 2,800</p>
              
            </div>
          </div>
         

        </div>
      </div>
     </div>  -->
  </div>
</template>
<script>
  // import Card from 'src/components/Cards/Card.vue'
import axios from 'axios'
  export default {
    data(){
      return{
        posts:[],
        baseUrl: process.env.MAIN_API ? process.env.MAIN_API : "",
      }
    },
    // components: {
    //   Card
    // },
    // data () {
    //   return {
    //     user: {
    //       company: 'Light dashboard',
    //       username: 'michael23',
    //       email: '',
    //       firstName: 'Mike',
    //       lastName: 'Andrew',
    //       address: 'Melbourne, Australia',
    //       city: 'melbourne',
    //       country: 'Australia',
    //       postalCode: '',
    //       aboutMe: `Lamborghini Mercy, Your chick she so thirsty, I'm in that two seat Lambo.`
    //     }
    //   }
    // },
    methods: {
      updateProfile () {
        alert('Your data: ' + JSON.stringify(this.user))
      }
    },
   mounted(){
  //   
    // axios.defaults.headers.common['Access-Control-Allow-Origin'] = "https://prosperc40.pythonanywhere.com/"
    //  const headers = { 'Authorization': 'Bearer ' +'6124bc0794931a48a4665935619ee039bb7be277','Content-Type': 'application/json', };
      axios.get('https://prosperc40.pythonanywhere.com/products',{
      headers: {
    'Authorization': 'Token ' + '6124bc0794931a48a4665935619ee039bb7be277'
  }}
      )
  .then(response => {
    console.log(response);
    this.posts=response.data

    console.log(this.posts)
    // Now check the structure of the response and ensure it has a 'protocol' property.
  })
  .catch(error => {
    console.error('Error fetching data:', error);
  })
    
    }
  
  }
  
   
    // async create(){
    //   try {
    //   const response = await axios.get();
    //   this.posts = response.data;
    //   console.log(this.posts)
    // } catch (error) {
    //   console.error(error);
    // }
    // }
   

</script>
<style>
.ge{
  font-size:12px !important;
  font-weight:bold;
}
.fr{
  font-size:11px !important;
}
.lu{
  width:15px;
  height:15px;
}
.fe{
  margin-top:-12px;
}
.bt-new{
  background-color:white;
  border:1px solid black;
  color:rgb(54, 54, 54);
  border-radius:20px;
  padding-left:10px;
  padding-right:10px;
  padding-top:5px;
  padding-bottom:5px;
}
.cc{
  overflow-x: hidden !important;
}

</style>