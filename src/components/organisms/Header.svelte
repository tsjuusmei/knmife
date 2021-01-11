<style>

	* {
		margin: 0;
		padding: 0;
	}

	h1 {
		font-family: "Roboto";
		text-transform: uppercase;
		font-size: 100px;
		font-weight: 500;
		margin: auto;
		z-index: 1000;
	}

	header {
		max-width: none;
		background-image: url("../images/bg.gray.svg");
		background-size: cover;
		text-align: center;
		height: 90%;
		display: flex;
		flex-direction: column;
		margin-bottom: -1%;
	}

	img {
		position: relative;
		width: 80px;
		bottom: 4vh;
		margin: 0 auto;
		animation: pulse 2s 3s ease-out infinite;
		z-index: 1000;
	}

	@keyframes pulse {
		0% {
			transform: none;
		}
		50% {
			transform: translateY(-0.5rem);
		}
		80% {
			transform: none;
		}
		100% {
			transform: none;
		}
	}
</style>

<header>
	<h1>How did COVID-19 <br /> affect the NO² emissions?</h1>
	<a href="#intro">
		<img src="../images/arrowdown.svg" class="bounce" alt="" />
	</a>
</header>
