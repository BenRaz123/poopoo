<template>
  <head>
  <link rel="stylesheet" href="styles.css">
    <link
      rel="stylesheet"
      href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@48,400,0,0"
    />
  </head>
  <!-- Navbar -->
  <NavBar />
  <!-- Main Body -->
  <MainBody />
</template>

<script setup>

import NavBar from "./components/navbar.vue";
import MainBody from "./components/mainbody.vue";

</script>

<style>

@import url("https://use.typekit.net/vup8xjj.css");

@media (prefers-color-scheme: light) {
	:root {
		--background-color: #cdf;
		--text-color: black;
		--nav-border-color: #abd;
		--card-background-color: rgba(0,0,0,.09);
		--card-border-color: rgba(0,0,0,.1)
	}
}

@media (prefers-color-scheme: dark) {
	:root {
		--background-color: #124;
		--text-color: white;
		--nav-border-color: #235;
		--card-background-color: rgba(255,255,255,.05);
		--card-border-color: rgba(255,255,255, 0.05)
	}
}

a {
	color: inherit
}

* {
	font-family: ff-nexus-sans, sans-serif;
}

p {
	font-size: 1.5rem;
}

img {
	max-width: 10rem;
	max-height: 10rem;
	margin-right: 1rem;
}

h1,h2, h3, h4, h5, h6, p {
	color:var(--text-color);
}

h1 {
	font-size: 3rem;
	font-family: ff-nexus-serif;
	font-weight: 100;
	line-height: 4rem;
}

*::before {
	transition: none !important
}

.navbar-item:hover {
	color: #5a5;
	transition-duration: 0s !important;
}

.nav-links-container {
	margin:0rem;
	color: var(--text-color);
	margin:none;
	display: flex;
}

.title-section {
	display:flex;
	flex-direction: row;
	column-gap: 2rem;
	background-color: var(--card-background-color);
	border: var(--card-border-color) 0.5rem solid;
	margin:1rem;
	padding: 1rem;
	border-radius: 2rem;
	justify-content: space-between;
	align-items: center;
}

.title-section-text {
	display: flex;
	flex-direction: column;
	margin:0rem;
	margin-left:1rem;
	padding:0rem;
}

#nav-title {
	font-weight: BOLD;
	color: #5a5;
	text-align: left;
	font-size: 1rem
}

.navbar > * >a {
	text-decoration: none;
	margin:0rem;
	padding:0rem;
}

.navbar {
	align-items: center;
	display: flex;
	position: fixed;
	top:0;
	width:100%;
	justify-content: space-between;
	flex-direction: row;
	background-color: var(--background-color);
	border-bottom: var(--nav-border-color) 2px solid;
	padding:0.25rem;
	filter: drop-shadow(0px 0px 0px #5a5);
	transition-duration: 1.25s;
}

.navbar:hover {
	filter: drop-shadow(0px 5px 10px #5a5);
	border: var(--background-color) 0px solid;
}

.navbar > * > * {
	color: var(--text-color);
	padding:0rem;
	margin:0rem
}

i {
  margin-right: 0.5rem;
}

.navbar-item {
	text-align: right;
	padding:0rem;
	margin:1rem
}

body {
	padding-top: 4rem;
	margin:0px;
	background-color: var(--background-color)
}

@media only screen and (max-width:700px) {
	.title-section {
		flex-direction: column-reverse;
	}
}

@media only screen and (max-width:700px) {
	.icon-text {
		display:none;
	}

	i {
		font-size:2rem;
	}
}

@media only screen and (max-width:400px) {
	i {
		font-size: 1rem;
	}

	.nav-links-container {
		column-gap: 0rem;
	}
}

@media only screen and (min-width: 1300px) {
	p {
		width: 50vw
	}
}

</style>
