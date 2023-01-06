<script>
	import { page } from '$app/stores';
	import logo from '$lib/images/svelte-logo.svg';
</script>

<header>
	<nav>
		<ul>
			<li><strong>Focus Pocus</strong></li>

		</ul>
		<ul>
			<li>
				<button data-target="modal-example" onClick="toggleModal(event)">
				Add Task
			</button>
		</li>
		</ul>
	</nav>

	<dialog id="modal-example">
		<article>
			<a href="#close"
				aria-label="Close"
				class="close"
				data-target="modal-example"
				onClick="toggleModal(event)">
			</a>
			<h3>Confirm your action!</h3>
			<p>
				Cras sit amet maximus risus. 
				Pellentesque sodales odio sit amet augue finibus pellentesque. 
				Nullam finibus risus non semper euismod.
			</p>
			<footer>
				<a href="#cancel"
					role="button"
					class="secondary"
					data-target="modal-example"
					onClick="toggleModal(event)">
					Cancel
				</a>
				<a href="#confirm"
					role="button"
					data-target="modal-example"
					onClick="toggleModal(event)">
					Confirm
				</a>
			</footer>
		</article>
	</dialog>

</header>



<style>
	.nav {
		vertical-align: middle;
		text-align: center;
	}
</style>



