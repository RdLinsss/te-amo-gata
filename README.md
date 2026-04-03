:root {
    --primary-color: #f7d7da;
    --accent-color: #d81b60;
    --text-color: #4a4a4a;
    --bg-color: #fff;
    --light-bg: #fdfdfd;
    --font-poppins: 'Poppins', sans-serif;
    --font-dancing: 'Dancing Script', cursive;
    --font-vibes: 'Great Vibes', cursive;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: var(--font-poppins);
    background-color: var(--bg-color);
    color: var(--text-color);
    line-height: 1.6;
    overflow-x: hidden;
}

.container {
    max-width: 1000px;
    margin: 0 auto;
    padding: 0 20px;
}

header {
    background-color: var(--light-bg);
    padding: 80px 0;
    border-bottom: 2px solid #f2f2f2;
}

.header-flex {
    display: flex;
    align-items: center;
    gap: 40px;
}

.header-text {
    flex: 1.2;
}

header h1 {
    font-family: var(--font-vibes);
    font-size: 5rem;
    color: var(--accent-color);
    margin-bottom: 10px;
}

.tagline {
    font-size: 1.1rem;
    font-weight: 300;
    text-transform: uppercase;
    letter-spacing: 3px;
    color: #888;
}

.header-photo {
    flex: 1;
    display: flex;
    justify-content: flex-end;
}

.header-photo img {
    max-width: 100%;
    height: auto;
    border-radius: 20px;
    box-shadow: 15px 15px 50px rgba(0,0,0,0.1);
    transform: rotate(2deg);
}

.intro {
    text-align: center;
    padding: 100px 0;
    background-color: var(--bg-color);
}

.intro h2 {
    font-family: var(--font-dancing);
    font-size: 3rem;
    color: var(--accent-color);
    margin-bottom: 30px;
}

.timeline {
    padding-bottom: 100px;
}

.timeline-item {
    display: flex;
    align-items: flex-start;
    gap: 40px;
    margin-bottom: 80px;
}

.timeline-item.reversed {
    flex-direction: row-reverse;
}

.timeline-photo {
    flex: 1;
}

.timeline-photo img {
    width: 100%;
    height: auto;
    border-radius: 15px;
    box-shadow: 0 10px 30px rgba(0,0,0,0.05);
}

.timeline-text {
    flex: 1;
}

.timeline-text h3 {
    font-size: 1.8rem;
    color: var(--accent-color);
    margin-bottom: 15px;
}

.sub-photos {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 15px;
    margin-top: 20px;
}

.sub-photos img {
    width: 100%;
    height: auto;
    border-radius: 10px;
}

.dedication {
    background-color: var(--light-bg);
    padding: 80px 40px;
    border-radius: 30px;
    border: 3px dashed var(--primary-color);
    text-align: center;
    margin-bottom: 100px;
}

.signature {
    font-family: var(--font-vibes);
    font-size: 3rem !important;
    color: var(--accent-color);
}

footer {
    text-align: center;
    padding: 40px 0;
    background-color: #222;
    color: white;
}

@media (max-width: 768px) {
    .header-flex { flex-direction: column-reverse; text-align: center; }
    header h1 { font-size: 3.5rem; }
    .timeline-item, .timeline-item.reversed { flex-direction: column; }
}
