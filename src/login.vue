<template>
    <el-form ref="form" :model="form" label-width="80px">
        <h2>登录系统</h2>
        <el-form-item label="账号:">
            <el-input v-model="form.name"></el-input>
        </el-form-item>
        <el-form-item label="密码:">
            <el-input v-model="form.password"></el-input>
        </el-form-item>
        <el-form-item>
            <el-button type="primary" @click="onSubmit">登录</el-button>
        </el-form-item>
    </el-form>
</template>
<script>
    export default {
        data() {
            return {
                form: {
                    name: '',
                    region: '',
                    date1: '',
                    date2: '',
                    delivery: false,
                    type: [],
                    resource: '',
                    desc: ''
                }
            }
        },
        methods: {
            onSubmit() {
                alert("欢迎登录!")
            }
        }
    }
</script>

<style>
    form {
        background-color: white;
        width: 20%;
        height: 250px;
        margin: 300px auto;
        border-radius: 8px;
        padding: 20px;
    }

    h2 {
        text-align: center;
    }

</style>
