<template>
    <body id="login-body">
        <meta content="width=50%">
        <div class="title">
            <h1> Topi Login Page </h1>
            <p><i>Welcome back!</i></p>
        </div>

        <div >
            <form action="#" method="post">

                <div class="container">
                    <label for="username"><b>Username</b></label>
                    <input type="text" placeholder="Enter Your Username" name="username" required>
                    <label for="password"><b>Password</b></label>
                    <input type="password" placeholder="Enter Your Password" name="password" required>
                    
                </div>

                <div class ="remember">
                    <button type="submit" class="login">Login</button>
                    <label>
                        <input type="checkbox" checked="checked" name="remember"> <i>Remember me</i>
                    </label>
                </div>

                <div class="container" style="background-color:#04AA6D">
                    <button type="submit" class="cancel">Cancel</button>
                    <span class="password"> <router-link to="./forgot.vue">Forgot password? </router-link>
                    </span>
                </div>

                <div class="list-links">
                    <ul><a href="#">Home</a></ul>
                    <ul><a href="?#/about">About</a></ul>
                </div>

            </form>
            </div>
    </body>
</template>

<script lang="ts">
    
</script>

<style>

.list-links{
    padding: 7px 85px;
    margin: 0px;
    background: #04AA6D;
    color:beige;
    text-align: right;
}
.title {
    margin: 0 auto;
    width: 600px;
    font-display: italic;
}
body {
    background: beige;
    /* //background-image: url(background.jpg); */
    background-size:auto;
    max-width: 70;
    scale: 10;

    
}
form {
    border: 5px groove #04AA6D;
    margin: 0 auto;
    width: 600px;
    text-align: center;
    background-color: bisque;
    
    }

input[type=text], input[type=password] {
    width: 100%;
    padding: 15px 10px ;
    margin: 10px 0;
    display: inline-block;
    border: 5px solid #ccc;
    box-sizing: border-box;
}

.container {
    padding: 40px;
}
.remember {
    padding: 10px 50px;
}

.login {
    transition-duration: 0.4s;
    box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2), 0 6px 20px 0 rgba(0,0,0,0.19);
    background-color: #04AA6D;
    color: white;
    padding: 14px 20px;
    margin: 8px 10px;
    cursor: pointer;
    width: 50%;
    border-radius: 12px;

}
.login:hover {
    opacity: 0.8;
    /* color: white; */
    box-shadow: 0 12px 16px 0 rgba(0,0,0,0.24), 0 17px 50px 0 rgba(0,0,0,0.19);
}

span.password {
    float: right;
    padding-top: 16px;
}
.cancel {
     transition-duration: 0.4s;
    box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2), 0 6px 20px 0 rgba(0,0,0,0.19);
    border-radius: 12px;
    transition-duration: 0.4s;
    width: auto;
    padding: 10px 18px;
    background-color: goldenrod;
    float:left;
}
.cancel:hover {
     opacity: 0.8;
    /* color: white; */
    box-shadow: 0 12px 16px 0 rgba(0,0,0,0.24), 0 17px 50px 0 rgba(0,0,0,0.19);
}
</style>