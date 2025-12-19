<!doctype html>
<html lang="pt-BR">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Stream Panel</title>
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/github-markdown-css@5.6.1/github-markdown.min.css">
  <style>
    body { max-width: 980px; margin: 0 auto; padding: 24px; }
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
