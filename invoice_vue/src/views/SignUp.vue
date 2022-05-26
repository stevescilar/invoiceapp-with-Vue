<template>
    <div class="page-signup">
        <div class="columns">
            <div class="column is-4 is-offset-4">
                <h1 class="title">Sign Up</h1>

                <form @submit.prevent="submitForm">
                    <div class="field">
                        <label for="">E-mail</label>
                        <div class="control">
                            <input type="email" name="username" id="" class="input" v-model="username">
                        </div>
                    </div>
                    <div class="field">
                        <label for="">Password</label>
                        <div class="control">
                            <input type="password" name="password" id="" class="input" v-model="password">
                        </div>
                    </div>
                    <div class="notification is-danger" v-if="errors.length">
                    <p v-for="error in errors" v-bind:key="error">
                        {{ error }}
                    </p>
                    </div>
                </form>
            </div>
        </div>
    </div>
</template>

<script>
export default{
    name:'SignUp'
}
</script>