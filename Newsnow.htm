<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8"/>
  <meta name="viewport" content="width=device-width,initial-scale=1"/>
  <title>📰 Live News—English | हिंदी | অসমীয়া</title>
  <style>
    body { font-family: sans-serif; margin: 0; background: #f4f4f4; }
    nav { display: flex; justify-content: center; background: #333; }
    nav button { padding: 0.75rem 1.5rem; border: none; color: #fff; background: none; cursor: pointer; }
    nav button.active { background: #555; }
    .container { max-width: 900px; margin: 1rem auto; padding: 0 1rem; }
    .card { background: #fff; margin: 1rem 0; padding: 1rem; border-radius: 8px; display: flex; gap: 1rem; box-shadow: 0 2px 6px rgba(0,0,0,0.1); }
    .card img { width: 120px; height: 80px; object-fit: cover; border-radius: 4px; }
    .details { flex: 1; }
    .details h3 { margin: 0 0 0.25rem; font-size: 1.1rem; }
    .details p { margin: 0 0 0.5rem; color: #555; }
    .details a { color: #0077cc; text-decoration: none; font-weight: bold; }
  </style>
</head>
<body>

<nav>
  <button data-lang="en" class="active">English</button>
  <button data-lang="hi">हिंदी</button>
  <button data-lang="as">অসমীয়া</button>
</nav>

<div class="container" id="news-container">Loading news...</div>

<script>
  const tabs = document.querySelectorAll('nav button');
  const container = document.getElementById('news-container');

  tabs.forEach(btn => {
    btn.addEventListener('click', () => {
      tabs.forEach(b => b.classList.remove('active'));
      btn.classList.add('active');
      loadNews(btn.dataset.lang);
    });
  });

  async function loadNews(lang) {
    container.innerHTML = 'Loading...';
    try {
      const key = 'YOUR_NEWSDATA_API_KEY'; // replace with your key
      const url = `https://newsdata.io/api/1/news?apikey=${key}&language=${lang}`;
      const res = await fetch(url);
      const data = await res.json();
      const news = data.results || [];
      if (!news.length) {
        container.innerHTML = '<p>No news available.</p>';
        return;
      }
      container.innerHTML = '';
      news.slice(0, 10).forEach(item => {
        const card = document.createElement('div');
        card.className = 'card';
        card.innerHTML = `
          ${item.image ? `<img src="${item.image}" alt="News Image">` : ''}
          <div class="details">
            <h3>${item.title}</h3>
            <p>${item.description?.split('. ').slice(0,2).join('. ')}...</p>
            <a href="${item.link}" target="_blank">Read more →</a>
          </div>`;
        container.appendChild(card);
      });
    } catch (e) {
      container.innerHTML = '<p>Error loading news. Please try again later.</p>';
      console.error(e);
    }
  }

  loadNews('en');
</script>

</body>
</html>
