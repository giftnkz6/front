<template>
    <div class="container w-50">
        <div class="row">
            <div id="form" class="container justify-content-center">
                <form class="form container mt-3" action="https://formspree.io/f/mrgdkjgy" method="POST">
                    <h1>Contact Us</h1>
                    <div class="form-floating mb-4">
                        <input type="text" class="form-control" name="name" placeholder="Enter your name" id="floatingInput" required>
                        <label for="floatingInput">Enter your name</label>
                    </div>
                    <div class="form-floating mb-4">
                        <input type="text" class="form-control" name="surname" placeholder="Enter your surname" id="floatingInput" required>
                        <label for="floatingInput">Enter your surname</label>
                    </div>
                    <div class="form-floating mb-4">
                        <input type="email" class="form-control" placeholder="Enter your email" id="floatingInput" required>
                        <label for="floatingInput">Enter your email</label>
                    </div>
                    <div class="form-floating mb-4">
                        <textarea class="form-control" placeholder="Leave a comment here" id="floatingTextarea" required></textarea>
                        <label for="floatingTextarea">Write me a message</label>
                    </div>
                    <div class="mb-4">
                        <button class="btn btn-outline-info">Submit</button>
                    </div>
                </form>
            </div>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style scoped>
    .form-floating #floatingTextarea{
        height: 6rem
    }
    h1{
        margin-top: 2rem;
        margin-bottom: 2rem;
        text-shadow: 2px 1px white;
    }
    #form{
        width: 35rem;
        box-shadow: 0 0 25px lightgrey;
        margin-top: 2rem;
        margin-bottom: 2rem;
        background-color: white; 
        /* background-color: white;  */
    }

    /* @media screen and (max-width: 750px) {
    #form{
        min-width: 25rem;
    }
} */
    @media screen and (max-width: 390px) {
    #form{
        min-width: 14rem;
    }
}
@media screen and (max-width: 300px) {
    #form{
       border: none;
}
@media screen and (max-width: 530px) {
    #form{
        min-width: 15rem;
    }
}
@media screen and (max-width: 380px) {
    #form{
        min-width: 13rem;
    }
}
@media screen and (max-width: 426px) {
    #form{
        min-width: 18rem;
    }
}
@media screen and (max-width: 360px) {
    #form{
        min-width: 10rem;
    }
}

@media screen and (max-width: 340px) {
    #form{
        min-width: 14rem;
    }
}
@media screen and (max-width: 300px) {
    /* .row {

        height: 80vh;

    } */

    #form{
        min-width: 12rem;
        /* position: absolute; */
        /* left: 0%;  */
        margin-right: 3rem;

    }
}
}
</style>