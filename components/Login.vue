<template>
    <div class="d-flex justify-content-center align-items-center" style="height: 100vh;">
        <div class="card card-content">
            <div>
                <img src="../assets/img/header-login.png" class="icon-header" alt="Header Login" />
                <img src="../assets/img/logo.png" style="width:100px;" class="pt-3" alt="Header Login" />
            </div>
            <div class="card-body">
                <div class="py-3">
                    <div class="tittle-page">Login</div>
                    <div class="tittle-desc">Please sign in to continue</div>
                </div>
                <div class="py-3">
                    <div>User ID</div>
                    <input type="text" class="py-2 input-from" placeholder="User ID" />
                </div>
                <div class="py-3">
                    <div>Password</div>
                    <input type="password" class="py-2 input-from" placeholder="Password" />
                </div>
                <div class="py-2 d-flex justify-content-end" @click="showModal = true">
                    <button class="btn btn-login">LOGIN</button>
                </div>
                <div class="d-flex justify-content-center pt-5">
                    Don't have account? <div class="signUp-text">Sign Up</div>
                </div>
            </div>
        </div>
    </div>
</template>

<style>
body {
    background-color: #ec462d9d;
    font-family: Arial, Helvetica, sans-serif;
}

.icon-header {
    width: 100px;
    border-top-left-radius: 10px;
}

.tittle-page {
    font-size: 25px;
    font-weight: bold;
}

.signUp-text {
    padding-left: 5px;
    color: #EE684A;
    cursor: pointer;
}

.signUp-text:hover {
    text-decoration: underline;
}

.btn-login {
    background: #6338A1;
    color: #FFF;
    font-weight: 600;
    border-radius: 17px;
    padding: 8px 27px;
}

.tittle-desc {
    font-size: 15px;
    font-weight: 500;
}

input::placeholder {
    font-style: italic;
    opacity: .5;
    color: rgb(177, 170, 170);
}

.card-content {
    width: 22rem;
    border-radius: 12px;
}

.input-from {
    border: none;
    border-bottom: 1px solid;
    width: 100%;
}

.input-from:focus {
    outline: none;
}
</style>

<script>
export default {
    name: 'LoginPage'
}
</script>