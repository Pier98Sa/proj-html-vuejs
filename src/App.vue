<template>
  <div id="app">
    <MyHeader :links="links" />
    <MyHero />
    <MyMain :instructors="instructors" />
    <MyFooter :courses="courses"/>
    
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue'
import MyHero from './components/MyHero.vue'
import MyMain from './components/MyMain.vue'
import MyFooter from './components/MyFooter.vue'

export default {
  name: 'App',
  components: {
    MyHeader,
    MyHero,
    MyMain,
    MyFooter,
  },
  data(){
    return{
      links: [
        {
            text: "Home",
            url: "#",
            new: false
        },
        {
            text: "About",
            url: "#",
            new: false
        },
        {
            text: "Prices",
            url: "#",
            new: false
        },
        {
            text: "Courses",
            url: "#",
            new: true
        },
        {
            text: "Locations",
            url: "#",
            new: false
        },
        {
            text: "Blog",
            url: "#",
            new: false
        }
      ],
      courses:[
        {
            name: 'Pass Plus',
            link: '#'
        },
        {
            name: 'Intensive Course',
            link: '#'
        },
        {
            name: 'Automatic',
            link: '#'
        },
        {
            name: 'Instructor Training',
            link: '#'
        }
      ],
      instructors: [
                {
                    name: 'Mike Hart',
                    photo: '-mikehart.jpg',
                    description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.'
                },
                {
                    name: 'John Smith',
                    photo: '-johnsmith.jpg',
                    description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.'
                },
                {
                    name: 'Angela Hart',
                    photo: '-angelahart.jpg',
                    description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.'
                }
            ]

    }
  }
}
</script>

<style lang="scss">
  @import './style/general.scss';
  @import '~@fortawesome/fontawesome-free/css/all.css';
  @import './style/variables.scss';
  @import url('https://fonts.googleapis.com/css2?family=Mulish:ital,wght@0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&family=Open+Sans:wght@300;400;600&display=swap');

  #app{
    font-family: 'Mulish', sans-serif;
  }

  //rule for button
  .ms_btn{
    border-radius: 16px;
    border: none;
    font-size: 12px;
    text-transform: uppercase;
    padding: 8px 16px;
    
  }
  //rule for green button
  .ms_btn-green{
    background-color: $primaryColorButton;
    color: $tertiaryColorButton;
    
    &:hover{
      background-color: $secondaryColorButton;
    }
  }

  //rule for grey button
  .ms_btn-grey{
    color: $quaternaryColorButton;
    border: 2px solid $quaternaryColorButton;
    background-color: transparent;

    &:hover{
    color: $primaryColorButton;
    border-color: $primaryColorButton;
    }
  }
  //rule for offset
  .ms_offset{
    margin-top: -30px;
    z-index: 998;
  }

  .ms_offset-2{
    margin-top: -50px;
    z-index: 998;
  }

  .ms_offset-3{
    margin-top: -1px;
  }
  .ms_offset-4{
    margin-top: -120px;
  }

  .ms_offset-5{
    margin-bottom: -70px;
    z-index: 998;
  }
</style>
 