<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    
</head>
<body>

<h1>VKrDownloader</h1>
<p>
    Video Downloader by Vijay Kumar 
    <a href="https://instagram.com/theofficialvkr">@TheOfficialVKr</a> 
</p>

<p>Download videos from:</p>
<ul>
    <li>YouTube</li>
    <li>Facebook</li>
    <li>Twitter</li>
    <li>Instagram (Reels)</li>
    <li>TikTok</li>
    <li>1000+ other websites in all audio/video quality options</li>
</ul>

<h2>API Documentation</h2>

<p>With the VKrDownloader API, you can programmatically download videos from supported sites.</p>

<h3>API Endpoint</h3>
<pre><code>GET https://vkrdownloader.vercel.app/server/?vkr=VIDEO_URL</code></pre>

<h3>Request Parameters</h3>
<ul>
    <li><strong>vkr</strong> (string) - <em>Required</em>. The URL of the video you want to download.</li>
</ul>

<h3>Authentication</h3>
<p>You must pass an API key to authenticate your requests. The API key can be passed in two ways:</p>

<ul>
    <li><strong>Query string</strong>: Append <code>api_key=YOUR_API_KEY</code> to the URL.</li>
    <li><strong>HTTP Header</strong>: Include the API key using the <code>x-api-key</code> header in your request.</li>
</ul>

<h3>Example Request (Query String)</h3>
<pre><code>curl "https://vkrdownloader.vercel.app/server/?api_key=YOUR_API_KEY&vkr=https://www.youtube.com/watch?v=dQw4w9WgXcQ"
</code></pre>

<h3>Example Request (Header)</h3>
<pre><code>curl -X POST https://vkrdownloader.vercel.app/server/ \
-H "x-api-key: YOUR_API_KEY" \
-d "vkr=https://www.youtube.com/watch?v=dQw4w9WgXcQ"
</code></pre>

<h3>Example Response</h3>
<pre><code>{
  "title": "Sample Video",
  "url": "https://video-download-link.com/file.mp4",
  "thumbnail": "https://img.youtube.com/sample_thumbnail.jpg",
  "formats": [
    {
      "format_id": "18",
      "resolution": "360p",
      "ext": "mp4",
      "filesize": "10 MB"
    },
    {
      "format_id": "22",
      "resolution": "720p",
      "ext": "mp4",
      "filesize": "25 MB"
    }
  ]
}
</code></pre>

<h3>Error Handling</h3>
<ul>
    <li><strong>401 Unauthorized</strong> - Returned if the API key is missing or invalid.</li>
    <li><strong>400 Bad Request</strong> - If the video URL is invalid or missing.</li>
    <li><strong>500 Internal Server Error</strong> - If an unexpected error occurs while processing the request.</li>
</ul>

<h3>API Key</h3>
<p>To access the VKrDownloader API, you need an API key. You can pass it in the query string or the request header as <code>x-api-key</code>.</p>

<h4>Example (Query String)</h4>
<pre><code>https://vkrdownloader.vercel.app/server/?api_key=YOUR_API_KEY&vkr=https://www.youtube.com/watch?v=dQw4w9WgXcQ</code></pre>

<h4>Example (Header)</h4>
<pre><code>curl -X POST https://vkrdownloader.vercel.app/server/ \
-H "x-api-key: YOUR_API_KEY" \
-d "vkr=https://www.youtube.com/watch?v=dQw4w9WgXcQ"
</code></pre>

<p>For more information about obtaining an API key, please 
<a href="mailto:contactvkr@yahoo.com">contact us</a>.</p>

<hr>

<h2>How To Install</h2>
<ol>
    <li>Upload zip files to your server or hosting platform.</li>
    <li>Unzip the file in your file manager.</li>
    <li>This project works on almost all free/paid hosting, so don't worry about specific requirements.</li>
    <li>That's it! Open your site, and VKrDownloader will start working immediately.</li>
</ol>

<hr>

<h2>Demo</h2>
<p><a href="https://theofficialvkr.github.io/VKRdownloader/">https://theofficialvkr.github.io/VKRdownloader/</a></p>

<hr>

<h2>Updates</h2>
<p>Check all updates here:  
<a href="https://github.com/theofficialvkr/VKRdownloader/blob/main/updates.md">Updates Page</a></p>

<hr>

<h2>Need Help?</h2>
<p>Contact me for any kind of help:</p>
<ul>
    <li><strong>Email</strong>: <a href="mailto:contactvkr@yahoo.com">contactvkr@yahoo.com</a></li>
    <li><strong>Instagram</strong>: <a href="https://instagram.com/theofficialvkr">@theofficialvkr</a></li>
    <li><strong>Twitter</strong>: <a href="https://twitter.com/theofficialvkr">@theofficialvkr</a></li>
    <li><strong>Facebook</strong>: <a href="https://facebook.com/theofficialvkr">@theofficialvkr</a></li>
    <li><strong>Telegram</strong>: <a href="https://t.me/theofficialvkr">@theofficialvkr</a></li>
</ul>

<hr>

<h2>Support Me</h2>
<p>If you find this helpful, consider supporting me!</p>
<br>
<a href="https://www.paypal.com/ncp/payment/4C9YTYAMKYVZS">
    <img src="https://www.paypalobjects.com/images/Debit_Credit_APM.svg">
</a>
<br>
<a href="https://www.buymeacoffee.com/theofficialvkr">
    <img src="https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=&slug=theofficialvkr&button_colour=BD5FFF&font_colour=ffffff&font_family=Cookie&outline_colour=000000&coffee_colour=FFDD00">
</a>

<hr>

<h2>At Last, Remember</h2>
<p>I am not the Developer 👍</p>

</body>
</html>
