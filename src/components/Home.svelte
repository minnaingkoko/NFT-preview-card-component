<main class="home">
	<div class="container">
		<div class="card_img">
			<img class="equilibrium" src="/images/image-equilibrium.jpg" alt="" />
			<div class="overlay" />
			<img class="view" src="/images/icon-view.svg" alt="" />
		</div>
		<h1 class="heading">Equilibrium #3429</h1>
		<div class="text">Our Equilibrium collection promotes balance and calm.</div>
		<div class="row">
			<div class="left">
				<img class="ether" src="/images/icon-ethereum.svg" alt="" />
				<div class="value">0.041ETH</div>
			</div>
			<div class="right">
				<img class="clock" src="/images/icon-clock.svg" alt="" />
				<div class="date">3 days left</div>
			</div>
		</div>
		<div class="line" />
		<div class="profile">
			<div class="circle">
				<img class="avater" src="/images/image-avatar.png" alt="" />
			</div>
			<div class="profile_name">
				Creation of <div class="hl">Jules Wyvern</div>
			</div>
		</div>
	</div>
</main>

<style>
	.home {
		@apply w-screen h-screen flex justify-center items-center bg-[#0d192b];
	}
	.container {
		@apply w-[350px] h-[600px] rounded-[16px] p-[24px] bg-[#14253d] flex flex-col;
		box-shadow: 16px 24px #0c1727, -16px 24px #0c1727;
	}
	.card_img {
		@apply w-[302px] h-[302px] relative rounded-[8px] cursor-pointer;
	}
	.card_img:hover .overlay {
		@apply opacity-[0.5];
	}
	.card_img:hover .view {
		@apply block;
	}
	.equilibrium {
		@apply w-[100%] h-[100%] rounded-[8px];
	}
	.overlay {
		@apply absolute top-[0] left-[0] w-[100%] h-[100%] opacity-[0] duration-300 rounded-[8px] bg-[#00fff7];
	}
	.view {
		@apply hidden duration-300 absolute top-[50%] left-[50%] translate-x-[-50%] translate-y-[-50%];
	}
	.heading {
		@apply text-[#ffffff] text-[24px] font-semibold mt-[24px] cursor-pointer duration-300;
	}
	.heading:hover {
		@apply text-[#00fff7];
	}
	.text {
		@apply text-[#8bacda] text-[18px] mt-[18px] mb-[18px];
	}
	.row {
		@apply flex flex-row justify-between;
	}
	.left,
	.right {
		@apply flex flex-row gap-[6px] items-center;
	}
	.ether {
		@apply w-[11px] h-[18px];
	}
	.clock {
		@apply w-[17px] h-[17px];
	}
	.value {
		@apply text-[17px] font-light text-[#00fff7];
	}
	.date {
		@apply text-[17px] font-light text-[#8bacda];
	}
	.line {
		@apply w-[100%] h-[1px] bg-[#2f415b] mt-[16px] mb-[16px];
	}
	.profile {
		@apply flex flex-row items-center;
	}
	.circle {
		@apply flex justify-center items-center w-[34px] h-[34px] bg-[#ffffff] rounded-[50%] mr-[16px];
	}
	.avater {
		@apply w-[32px] h-[32px];
	}
	.profile_name {
		@apply flex flex-row gap-[6px] text-[#8bacda] text-[16px];
	}
	.hl {
		@apply text-[16px] text-[#ffffff] font-semibold cursor-pointer duration-300;
	}
	.hl:hover {
		@apply text-[#00fff7];
	}
	@media only screen and (max-width: 375px) {
		.container {
			width: calc(100% - 32px);
			padding: 24px;
		}
		.card_img {
			width: 100%;
			height: auto;
		}
		.equilibrium {
			width: 100%;
			height: auto;
		}
	}
</style>
