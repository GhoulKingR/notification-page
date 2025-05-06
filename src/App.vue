<script setup>
import MarkWebber from "./assets/images/avatar-mark-webber.webp";
import AngelaGray from "./assets/images/avatar-angela-gray.webp"
import JacobThompson from "./assets/images/avatar-jacob-thompson.webp";
import RizkyHasanuddin from "./assets/images/avatar-rizky-hasanuddin.webp";
import KimberlySmith from "./assets/images/avatar-kimberly-smith.webp";
import NathanPeterson from "./assets/images/avatar-nathan-peterson.webp";
import AnnaKim from "./assets/images/avatar-anna-kim.webp";
import Chess from "./assets/images/image-chess.webp";
</script>

<template>
	<header>
		<div>
			<h1 class="header">Notifications</h1>
			<span class="count">3</span>
		</div>

		<span class="mar"> Mark all as read </span>
	</header>

	<main>
		<div class="bubble unread">
			<img :src="MarkWebber" class="left" />
			<div class="body">
				<b>Mark Webber</b> reacted to your recent post
				<span>My first tournament today!</span>
				<span class="dot"></span>
				<small>1m ago</small>
			</div>
		</div>

		<div class="bubble unread">
			<img :src="AngelaGray" class="left" />
			<div class="body">
				<b>Angela Gray</b> followed you
				<span class="dot"></span>
				<small>5m ago</small>
			</div>
		</div>

		<div class="bubble unread">
			<img :src="JacobThompson" class="left" />
			<div class="body">
				<b>Jacob Thompson</b> has joined your group
				<span class="group">Chess Club</span>
				<span class="dot"></span>
				<small>1 day ago</small>
			</div>
		</div>

		<div class="bubble">
			<img :src="RizkyHasanuddin" class="left" />
			<div class="body">
				<b>Rizky Hasanuddin</b> sent you a private message
				<small>5 days ago</small>
				<p class="message">
					Hello,
					thanks for setting up the Chess Club. I've been a member for a few weeks now
					and I'm already having lots of fun and improving my game.
				</p>
			</div>
		</div>

		<div class="bubble">
			<img :src="KimberlySmith" class="left" />
			<div class="body">
				<b>Kimberly Smith</b> commented on your picture
				<small>1 week ago</small>
			</div>
			<img :src="Chess" class="right" />
		</div>

		<div class="bubble">
			<img :src="NathanPeterson" class="left" />
			<div class="body">
				<b>Nathan Peterson</b> reacted to your recent post
				<span>5 end-game strategies to increase your win rate</span>
				<small>2 weeks ago</small>
			</div>
		</div>

		<div class="bubble">
			<img :src="AnnaKim" class="left" />
			<div class="body">
				<b>Anna Kim</b> left the group
				<span class="group">Chess Club</span>
				<small>2 weeks ago</small>
			</div>
		</div>
		
	</main>
</template>

<style scoped>
* {
	font-family: pjs;
}

.dot {
	width: 8px;
	height: 8px;
	background-color: #F65552;
	display: inline-block;
	border-radius: 50%;
	margin-left: 6px;
}

header {
	display: flex;
	justify-content: space-between;
	align-items: center;
	padding-top: 24px;
	padding-left: 16px;
	padding-right: 16px;
	padding-bottom: 24px;
}

.header {
	font-weight: 800;
	font-size: 20px;
	line-height: auto;
	letter-spacing: 0px;
	margin-right: 9px;
}

.count {
	display: inline-block;
	font-size: 16px;
	font-weight: 800;
	line-height: auto;
	letter-spacing: 0px;
	padding-top: 1px;
	padding-bottom: 4px;
	padding-left: 11px;
	padding-right: 11px;
	background-color: #0a327b;
	color: #ffffff;
	border-radius: 6px;
}

.mar {
	font-weight: 500;
	color: #5e6778;
	font-size: 14px;
	line-height: auto;
	letter-spacing: 0px;
}

.bubble {
	display: flex;
	padding: 16px;
	padding-right: 26px;
	margin-left: 16px;
	margin-right: 16px;
	margin-bottom: 10px;
}

.bubble.unread {
	background-color: #f7fafd;
	border-radius: 8px;
}

.bubble img.left {
	height: 39px;
	width: 39px;
	margin-right: 13px;
}

.bubble img.right {
	height: 39px;
	width: 39px;
	margin-left: 27px;
}

.bubble .body {
	flex-grow: 1;
	font-weight: 500px;
	font-size: 14px;
	color: #5E6778;
}

.bubble b {
	font-weight: 800;
	line-height: auto;
	letter-spacing: 0px;
	color: #1C202B;
}

.bubble span {
	font-weight: 700;
}

.bubble span.group {
	color: #0A327B;
}

.bubble small {
	display: block;
	margin-top: 3px;
	color: #939CAD;
	font-weight: 500px;
	font-size: 14px;
}

.bubble p.message {
	display: block;
	margin-top: 12px;
	border-radius: 5px;
	border: 1px solid #DDE7EE;
	padding: 16px;
	font-size: 14px;
	font-weight: 500;
	color: #5E6778;
}
</style>
