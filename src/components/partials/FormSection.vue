<template>
    <section class="container-xl mb-3">
        <div class="row">

            <!--Description-->
            <div class="col-6 text pt-5">
                <h2 class="py-3 fw-bold ">Get Behind The Wheel</h2>
                <p class="fs-5">Lorem ipsum dolor sit amet consectetur, adipisicing elit.Nunc ultrices auctor sapien id cursus. Aliquam maximus turpis in vehicula semper. </p>
                <p class="ms_fs-7" >Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc ultrices auctor sapien id cursus. Aliquam maximus turpis in vehicula semper. Fusce et ultrices libero, at suscipit lacus. Sed vitae fringilla nibh. Nunc ultrices auctor sapien id cursus. Aliquam maximus turpis in vehicula semper. Fusce et ultrices libero, at suscipit lacus. Sed vitae fringilla nibh.</p>
            </div>

            <!--Form-->
            <div class="col-6 ms_offset px-5">
                <form >
                    <div class="p-5">
                        <h2 class="text-center pb-3">First Lesson Free!</h2>
                        <p class="text-center">When you make a block booking with us your first lesson is included free.</p>

                        <div class="position-relative">
                            <input class="pe-4" type="text" placeholder="Your Name*">
                            <img class="input-name-img" src="../../assets/image.png" alt="">
                        </div>
                        
                        <input type="email" placeholder="Email*">
                        <input type="text" placeholder="Telephone">
                        <input type="text" placeholder="Location">

                        <div class="d-flex justify-content-center mt-2">
                            <button type="submit" class="ms_btn ms_btn-green">Request a Callback</button>
                        </div>
                        
                    </div>
    
                </form>
            </div>
        </div>

    </section>
  
</template>

<script>
export default {
    name: 'FormSection',

}
</script>

<style lang="scss" scoped>
@import "../../style/variables.scss";
    .text{
        p{
            color: $tertiaryColorForm;   
        }
    }

    form{
        background-color: $secondaryColorForm;
        box-shadow: 1px 8px 10px #cdd1cd;
        border-radius: 12px;
        h2{
            color: $primaryColorForm;
        }
        p{
            color: $tertiaryColorForm;
            font-size: 16px;
        }
        input{
            width: 100%;
            font-size: 14px;
            padding: 8px;
            margin: 10px 0;
            border: 1px solid $tertiaryColorForm;
            border-radius: 6px;
            background-color: $quaternaryColorForm;
        }
    }

    // change placeholder text-color source: https://www.w3schools.com/howto/howto_css_placeholder.asp
    ::placeholder {
        color: $tertiaryColorForm;
        opacity: 1; /* Firefox */
    }

    :-ms-input-placeholder { /* Internet Explorer 10-11 */
        color: $tertiaryColorForm;
    }

    ::-ms-input-placeholder { /* Microsoft Edge */
        color: $tertiaryColorForm;
    }

    .ms_fs-7{
        font-size: 16px;
    }

    .input-name-img{
        position: absolute;
        top: 35%;
        right: 2%;
    }
</style>