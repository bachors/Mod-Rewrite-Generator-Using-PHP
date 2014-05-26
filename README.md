Mod-Rewrite-Generator-Using-PHP
===============================

Simple php function

Contoh

    http://www.domain.com/toko/tampil.php?jenis=barang&kategori=elektronik&nama=tv

Menjadi

    http://www.domain.com/barang/elektronik/tv.html

Kode htacces hasil generatenya:
<pre><code>
RewriteEngine On

RewriteRule ^([^/]*)/([^/]*)/([^/]*)\.html$ /toko/tampil.php?jenis=$1&kategori=$2&nama=$3 [L]
</code></pre>
