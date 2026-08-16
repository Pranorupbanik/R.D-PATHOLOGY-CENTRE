<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>R.D. Pathology Collection Centre</title>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

html{
    scroll-behavior:smooth;
}

body{
    font-family:Arial, Helvetica, sans-serif;
    background:#f7fbfa;
    color:#123238;
    line-height:1.6;
}

a{
    text-decoration:none;
    color:inherit;
}

.container{
    width:90%;
    max-width:1150px;
    margin:auto;
}

/* NAVBAR */

header{
    position:sticky;
    top:0;
    z-index:1000;
    background:rgba(255,255,255,.95);
    backdrop-filter:blur(12px);
    border-bottom:1px solid #dcebea;
}

nav{
    min-height:75px;
    display:flex;
    justify-content:space-between;
    align-items:center;
}

.logo{
    display:flex;
    align-items:center;
    gap:12px;
    font-weight:bold;
}

.logo-box{
    width:45px;
    height:45px;
    border-radius:14px;
    background:#087f83;
    color:white;
    display:flex;
    align-items:center;
    justify-content:center;
    font-weight:bold;
}

.logo small{
    display:block;
    color:#64787b;
    font-size:10px;
}

.nav-links{
    display:flex;
    gap:25px;
    align-items:center;
}

.nav-links a{
    font-size:14px;
    font-weight:bold;
    color:#50676a;
}

.nav-links a:hover{
    color:#087f83;
}

.call-btn{
    background:#087f83;
    color:white !important;
    padding:11px 18px;
    border-radius:25px;
}

/* HERO */

.hero{
    padding:85px 0 70px;
}

.hero-grid{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:60px;
    align-items:center;
}

.badge{
    display:inline-block;
    background:#e5f7f4;
    color:#087f83;
    padding:8px 15px;
    border-radius:30px;
    font-weight:bold;
    font-size:13px;
    margin-bottom:20px;
}

h1{
    font-size:clamp(42px,6vw,70px);
    line-height:1.05;
    letter-spacing:-3px;
    margin-bottom:22px;
}

.highlight{
    color:#087f83;
}

.hero p{
    color:#637477;
    font-size:18px;
    max-width:600px;
    margin-bottom:30px;
}

.buttons{
    display:flex;
    gap:12px;
    flex-wrap:wrap;
}

.btn{
    padding:14px 20px;
    border-radius:15px;
    font-weight:bold;
    display:inline-block;
    transition:.2s;
}

.primary{
    background:#087f83;
    color:white;
}

.primary:hover{
    transform:translateY(-3px);
}

.secondary{
    background:white;
    border:1px solid #d6e5e3;
}

.secondary:hover{
    transform:translateY(-3px);
}

.hero-image{
    position:relative;
}

.hero-image img{
    width:100%;
    border-radius:30px;
    box-shadow:0 25px 60px rgba(15,60,60,.15);
}

.rating{
    position:absolute;
    bottom:20px;
    left:-20px;
    background:white;
    padding:15px 20px;
    border-radius:18px;
    box-shadow:0 15px 40px rgba(0,0,0,.15);
}

.rating strong{
    display:block;
}

/* STATS */

.stats{
    background:white;
    border-top:1px solid #dcebea;
    border-bottom:1px solid #dcebea;
}

.stats-grid{
    display:grid;
    grid-template-columns:repeat(3,1fr);
}

.stat{
    text-align:center;
    padding:25px;
    border-right:1px solid #dcebea;
}

.stat:last-child{
    border-right:none;
}

.stat strong{
    display:block;
    font-size:24px;
    color:#087f83;
}

.stat span{
    font-size:13px;
    color:#6a7b7d;
}

/* SECTIONS */

section{
    padding:90px 0;
}

.section-title{
    text-align:center;
    margin-bottom:45px;
}

.section-title span{
    color:#087f83;
    font-weight:bold;
    font-size:13px;
    text-transform:uppercase;
    letter-spacing:2px;
}

.section-title h2{
    font-size:45px;
    margin-top:8px;
}

/* SERVICES */

.services{
    background:#073e41;
    color:white;
}

.services .section-title span{
    color:#7bded7;
}

.service-grid{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:18px;
}

.service{
    padding:30px;
    border:1px solid rgba(255,255,255,.12);
    background:rgba(255,255,255,.05);
    border-radius:25px;
    transition:.25s;
}

.service:hover{
    transform:translateY(-7px);
    background:rgba(255,255,255,.09);
}

.icon{
    font-size:30px;
    margin-bottom:20px;
}

.service h3{
    margin-bottom:8px;
}

.service p{
    color:#b7d1d0;
}

/* ABOUT */

.info-grid{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:25px;
}

.card{
    background:white;
    padding:30px;
    border-radius:27px;
    border:1px solid #dcebea;
    box-shadow:0 10px 30px rgba(0,0,0,.04);
}

.info{
    display:flex;
    gap:15px;
    padding:18px 0;
    border-bottom:1px solid #e1eceb;
}

.info:last-child{
    border-bottom:none;
}

.info-icon{
    width:43px;
    height:43px;
    background:#e6f7f4;
    color:#087f83;
    border-radius:13px;
    display:flex;
    justify-content:center;
    align-items:center;
    flex-shrink:0;
}

.info b{
    display:block;
}

.info span{
    color:#657578;
    font-size:14px;
}

/* REVIEW */

.review{
    background:linear-gradient(140deg,#e9f8f5,#ffffff);
}

.stars{
    color:#e5a914;
    font-size:24px;
    letter
