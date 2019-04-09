# vue-router-demo
### 组件使用

```
    <script src="../node_modules/vue/dist/vue.js"></script>
    <script src="./user/login.js"></script>
    <script src="./user/register.js"></script>
    <script>
        var app = new Vue({
            el: '#app',
            components: {
                loginForm,
                registerForm
            }
        })
    </script>
```

```
<login-form></login-form>
<register-form></register-form>
```

> 采用中划线的形式调用。

### 安装vue-router

```
npm install vue-router --save
```

#### 引入js

```
<script src="../node_modules/vue-router/dist/vue-router.js"></script>
```

#### 使用步骤

1.创建变量

```
        const router = new VueRouter({
            routes: [{
                    path: '/login',
                    component: loginForm
                },
                {
                    path: '/register',
                    component: registerForm
                }
            ]
        })
```

#### 2.引入变量使用路由

```
        var app = new Vue({
            el: '#app',
            components: {
                loginForm,
                registerForm
            },
            router
        })
```

