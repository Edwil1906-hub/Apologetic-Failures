<!DOCTYPE html>

<title>Apologetic Failures | Edwin Wilson</title>
<meta name="description" content="Apologetic Failures — An Apology for Failing as a Father — A Generational Curse by Edwin Wilson.">
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
    background:#080807;
    color:#eee9df;
    font-family:Georgia,"Times New Roman",serif;
    line-height:1.7;
}
nav{
    position:fixed;
    top:0;
    left:0;
    width:100%;
    padding:20px 6%;
    display:flex;
    justify-content:space-between;
    align-items:center;
    z-index:1000;
    background:linear-gradient(
        to bottom,
        rgba(8,8,7,.96),
        rgba(8,8,7,.55),
        transparent
    );
}
.logo{
    font-family:Arial,sans-serif;
    font-size:12px;
    letter-spacing:3px;
    font-weight:bold;
}
nav a{
    color:#eee9df;
    text-decoration:none;
    margin-left:22px;
    font-family:Arial,sans-serif;
    font-size:11px;
    letter-spacing:1.5px;
    text-transform:uppercase;
}
.hero{
    min-height:100vh;
    position:relative;
    display:flex;
    align-items:center;
    justify-content:center;
    text-align:center;
    overflow:hidden;
    padding:120px 7% 80px;
    background:
        radial-gradient(
            circle at 50% 38%,
            rgba(160,145,115,.13),
            transparent 32%
        ),
        radial-gradient(
            circle at 20% 80%,
            rgba(100,85,70,.08),
            transparent 35%
        ),
        #080807;
}
.hero:before{
    content:"";
    position:absolute;
    inset:30px;
    border:1px solid rgba(238,233,223,.16);
    pointer-events:none;
}
.hero:after{
    content:"";
    position:absolute;
    width:650px;
    height:650px;
    border-radius:50%;
    background:rgba(255,255,255,.025);
    filter:blur(80px);
    animation:pulse 8s ease-in-out infinite;
}
@keyframes pulse{
    0%,100%{
        transform:scale(.9);
        opacity:.35;
    }
    50%{
        transform:scale(1.1);
        opacity:.7;
    }
}
.hero-content{
    position:relative;
    z-index:2;
    max-width:950px;
}
.eyebrow{
    font-family:Arial,sans-serif;
    font-size:11px;
    letter-spacing:5px;
    text-transform:uppercase;
    color:#b8ad99;
    margin-bottom:28px;
}
h1{
    font-size:clamp(58px,11vw,145px);
    line-height:.86;
    font-weight:normal;
    letter-spacing:-5px;
    text-transform:uppercase;
    margin-bottom:35px;
}
.subtitle{
    max-width:680px;
    margin:auto;
    font-size:clamp(19px,3vw,28px);
    font-style:italic;
    color:#c8c0b3;
}
.author{
    margin-top:30px;
    font-family:Arial,sans-serif;
    font-size:12px;
    letter-spacing:5px;
    text-transform:uppercase;
    color:#a69b8b;
}
.enter{
    display:inline-block;
    margin-top:55px;
    padding:16px 30px;
    border:1px solid rgba(238,233,223,.45);
    color:#eee9df;
    text-decoration:none;
    font-family:Arial,sans-serif;
    font-size:11px;
    letter-spacing:3px;
    text-transform:uppercase;
    transition:.35s ease;
}
.enter:hover{
    background:#eee9df;
    color:#080807;
}
section{
    padding:120px 8%;
}
.section-label{
    font-family:Arial,sans-serif;
    font-size:10px;
    letter-spacing:4px;
    text-transform:uppercase;
    color:#9f9586;
    margin-bottom:22px;
}
.book{
    max-width:900px;
    margin:auto;
}
.book h2{
    font-size:clamp(38px,6vw,72px);
    line-height:1;
    font-weight:normal;
    margin-bottom:35px;
}
.book p{
    max-width:760px;
    color:#bdb5a9;
    font-size:18px;
    margin-bottom:25px;
}
.quote{
    margin-top:65px;
    padding:55px 0;
    border-top:1px solid rgba(238,233,223,.15);
    border-bottom:1px solid rgba(238,233,223,.15);
    font-size:clamp(25px,4vw,45px);
    line-height:1.25;
    font-style:italic;
}
.poetry{
    background:#0d0c0b;
}
.poetry h2{
    font-size:clamp(40px,6vw,70px);
    font-weight:normal;
    margin-bottom:50px;
}
.poem-grid{
    display:grid;
    grid-template-columns:repeat(2,1fr);
    gap:1px;
    background:rgba(238,233,223,.12);
}
.poem{
    background:#0d0c0b;
    padding:42px;
    min-height:190px;
    transition:.35s ease;
}
.poem:hover{
    background:#151310;
}
.poem-number{
    font-family:Arial,sans-serif;
    font-size:10px;
    letter-spacing:2px;
    color:#777064;
}
.poem h3{
    font-size:26px;
    font-weight:normal;
    margin:18px 0 10px;
}
.poem p{
    color:#999184;
    font-size:14px;
}
.statement{
    min-height:70vh;
    display:flex;
    align-items:center;
    justify-content:center;
    text-align:center;
    background:
        radial-gradient(
            circle,
            rgba(150,135,110,.08),
            transparent 55%
        );
}
.statement h2{
    max-width:1000px;
    font-size:clamp(38px,7vw,85px);
    line-height:1.05;
    font-weight:normal;
}
.author-section{
    max-width:900px;
    margin:auto;
}
.author-section h2{
    font-size:clamp(42px,6vw,75px);
    font-weight:normal;
    margin-bottom:30px;
}
.author-section p{
    color:#aaa195;
    font-size:18px;
    max-width:760px;
    margin-bottom:25px;
}
.closing{
    text-align:center;
    border-top:1px solid rgba(238,233,223,.1);
}
.closing h2{
    font-size:clamp(40px,7vw,90px);
    font-weight:normal;
    line-height:1;
}
.closing p{
    margin-top:25px;
    color:#938a7d;
    font-style:italic;
}
footer{
    padding:40px 8%;
    border-top:1px solid rgba(238,233,223,.1);
    display:flex;
    justify-content:space-between;
    color:#696359;
    font-family:Arial,sans-serif;
    font-size:10px;
    letter-spacing:2px;
    text-transform:uppercase;
}
@media(max-width:800px){
    nav{
        padding:18px 5%;
    }
    nav .links{
        display:none;
    }
    .hero{
        padding:110px 7% 70px;
    }
    .hero:before{
        inset:18px;
    }
    h1{
        font-size:17vw;
        letter-spacing:-2px;
    }
    .subtitle{
        font-size:20px;
    }
    section{
        padding:90px 7%;
    }
    .poem-grid{
        grid-template-columns:1fr;
    }
    .poem{
        padding:32px 25px;
    }
    footer{
        flex-direction:column;
        gap:15px;
        text-align:center;
    }
}
</style>
</head>
<body>
<nav>
    <div class="logo">APOLOGETIC FAILURES</div>
    <div class="links">
        <a href="#book">The Book</a>
        <a href="#poetry">Poetry</a>
        <a href="#author">The Author</a>
    </div>
</nav>
<header class="hero">
    <div class="hero-content">
        <div class="eyebrow">
            A Poetry Memoir by Edwin Wilson
        </div>
        <h1>
            Apologetic<br>
            Failures
        </h1>
        <div class="subtitle">
            An Apology for Failing as a Father —
            A Generational Curse
        </div>
        <div class="author">
            Edwin Wilson
        </div>
        <a href="#book" class="enter">
            Enter the Story ↓
        </a>
    </div>
</header>
<section id="book">
    <div class="book">
        <div class="section-label">
            The Book
        </div>
        <h2>
            A reckoning with
            what we inherit.
        </h2>
        <p>
            Some apologies are spoken.
            Others have to be written from
            the places where silence has lived
            for years.
        </p>
        <p>
            <em>Apologetic Failures</em> explores
            fatherhood, regret, love, accountability,
            and the generational wounds we carry
            long before we understand their names.
        </p>
        <div class="quote">
            “What if the things we inherit
            are not the things we have to become?”
        </div>
    </div>
</section>
<section id="poetry" class="poetry">
    <div class="section-label">
        Selected Works
    </div>
    <h2>
        The Poetry
    </h2>
    <div class="poem-grid">
        <article class="poem">
            <div class="poem-number">01</div>
            <h3>Apologetic Failures</h3>
            <p>
                An apology written from the
                uncomfortable space between
                love and accountability.
            </p>
        </article>
        <article class="poem">
            <div class="poem-number">02</div>
            <h3>Just 5 More Minutes</h3>
            <p>
                A meditation on time, absence,
                and the moments we wish we
                could have back.
            </p>
        </article>
        <article class="poem">
            <div class="poem-number">03</div>
            <h3>The Black Mind</h3>
            <p>
                An exploration of thought,
                identity, pressure, and survival.
            </p>
        </article>
        <article class="poem">
            <div class="poem-number">04</div>
            <h3>I Refuse to Change</h3>
            <p>
                What happens when love begins
                transforming the person you
                promised yourself you would remain?
            </p>
        </article>
        <article class="poem">
            <div class="poem-number">05</div>
            <h3>Permissive Will</h3>
            <p>
                Wrestling with choices,
                consequences, and the silence
                that follows them.
            </p>
        </article>
        <article class="poem">
            <div class="poem-number">06</div>
            <h3>The Black Child</h3>
            <p>
                Childhood, identity, inheritance,
                and the things children learn
                without being taught.
            </p>
        </article>
        <article class="poem">
            <div class="poem-number">07</div>
            <h3>Give Me Words</h3>
            <p>
                The desperate search for language
                when feelings become too large
                for ordinary speech.
            </p>
        </article>
        <article class="poem">
            <div class="poem-number">08</div>
            <h3>The Bitter Pill</h3>
            <p>
                Sometimes healing begins with
                swallowing the truth.
            </p>
        </article>
        <article class="poem">
            <div class="poem-number">09</div>
            <h3>Vision of Beauty</h3>
            <p>
                Finding beauty where pain once
                convinced us there was none.
            </p>
        </article>
        <article class="poem">
            <div class="poem-number">10</div>
            <h3>Nobody Stays Forever</h3>
            <p>
                Love, loss, memory, and the
                impermanence of human connection.
            </p>
        </article>
        <article class="poem">
            <div class="poem-number">11</div>
            <h3>Oxygen</h3>
            <p>
                When another person becomes
                the breath that awakens something
                long asleep.
            </p>
        </article>
    </div>
</section>
<section class="statement">
    <h2>
        There are wounds we inherit,
        and wounds we choose to end.
    </h2>
</section>
<section id="author">
    <div class="author-section">
        <div class="section-label">
            The Author
        </div>
        <h2>
            Edwin Wilson
        </h2>
        <p>
            Edwin Wilson writes from the
            uncomfortable space between memory
            and accountability.
        </p>
        <p>
            His words examine fatherhood,
            generational cycles, love, regret,
            identity, and the difficult process
            of becoming honest with oneself.
        </p>
        <p>
            <em>Apologetic Failures</em> is not an
            attempt to erase the past.
            It is an attempt to finally speak to it.
        </p>
    </div>
</section>
<section class="closing">
    <div class="section-label">
        A Poetry Memoir
    </div>
    <h2>
        Read what<br>
        had to be said.
    </h2>
    <p>
        Edwin Wilson
    </p>
</section>
<footer>
    <span>
        © 2026 Edwin Wilson
    </span>
    <span>
        Apologetic Failures
    </span>
</footer>
</body>
</html>
