<script>
import Router from 'svelte-spa-router'
import Autorization from './Autorization.svelte'
import StartDescription from './StartDescription.svelte'
import Recovery from './PasswordRecovery.svelte'
import Warning from './WarningEmail.svelte'
import NewPassword from './NewPassword.svelte'
import MainControllPage from './MainControllPage.svelte'
import PersonInform from './PersonInform.svelte'
import ChangePassword from './changePassword.svelte';
</script>

<Router routes={{
	"/": StartDescription,
	"/autorization": Autorization,
	"/recovery": Recovery,
	"/warningEmail": Warning,
	"/newpassword": NewPassword,
	"/maincontrollpage": MainControllPage,
	"/personinform": PersonInform,
	"/changepassword": ChangePassword
}} />

