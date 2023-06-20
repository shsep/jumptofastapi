<script>
  import Router from "svelte-spa-router"
  import Home from "./routes/Home.svelte"
  import Navigation from "./components/Navigation.svelte"
  import UserCreate from "./routes/UserCreate.svelte"
  import UserLogin from "./routes/UserLogin.svelte"
  import Detail from "./routes/Detail.svelte"
  import QuestionCreate from "./routes/QuestionCreate.svelte"

  const routes = {
    "/": Home,
    "/user-create": UserCreate,
    "/user-login": UserLogin,
    "/detail/:question_id": Detail,
    "/question-create": QuestionCreate,
  }
</script>

<Navigation />
<Router {routes} />