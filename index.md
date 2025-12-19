<!doctype html>
<html lang="pt-BR">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Stream Panel</title>
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/github-markdown-css@5.6.1/github-markdown.min.css">
<style>
  :root { color-scheme: dark; }

  body {
    max-width: 980px;
    margin: 0 auto;
    padding: 24px;
    background: #000;
  }

  /* Override do github-markdown-css */
  .markdown-body {
    background: #000 !important;
    color: #fff !important;
  }

  .markdown-body a { color: #7aa2ff !important; }
  .markdown-body hr { border-color: #333 !important; }

  .markdown-body code,
  .markdown-body pre {
    background: #111 !important;
    color: #fff !important;
  }

  .markdown-body blockquote {
    color: #ddd !important;
    border-left-color: #444 !important;
  }

  .markdown-body table th,
  .markdown-body table td {
    border-color: #333 !important;
  }

  .markdown-body h1, .markdown-body h2, .markdown-body h3,
  .markdown-body h4, .markdown-body h5, .markdown-body h6 {
    color: #fff !important;
    border-bottom-color: #222 !important;
  }
</style>

</head>
<body class="markdown-body">
  <div id="content">Carregando…</div>

  <script src="https://cdn.jsdelivr.net/npm/marked/marked.min.js"></script>
  <script>
    fetch('README.md')
      .then(r => r.ok ? r.text() : Promise.reject(r.status))
      .then(md => { document.getElementById('content').innerHTML = marked.parse(md); })
      .catch(err => { document.getElementById('content').textContent = 'Falha ao carregar README.md (' + err + ')'; });
  </script>
</body>
</html>
