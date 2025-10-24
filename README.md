<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Public File Storage Gallery</title>
    <style>
        body { font-family: sans-serif; max-width: 900px; margin: 40px auto; }
        .gallery { display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 20px; }
        .file-item { border: 1px solid #ddd; padding: 10px; text-align: center; }
        .file-item img, .file-item video { max-width: 100%; height: auto; display: block; margin: 0 auto 10px; border-radius: 5px; }
        .file-item .file-link { display: block; word-break: break-all; margin-top: 10px; }
    </style>
</head>
<body>

    <h1>Public Storage</h1>

    <div class="gallery">
        
        <div class="file-item">
            <h2>Photo</h2>
            <img src="/public/images/sunset_photo.jpg" alt="A photo of a sunset">
            <a href="/public/images/sunset_photo.jpg" class="file-link" download>Download Image</a>
        </div>

        <div class="file-item">
            <h2>Video</h2>
            <video controls preload="metadata" poster="/public/images/video_thumbnail.jpg">
                <source src="/public/videos/travel_clip.mp4" type="video/mp4">
                Your browser does not support the video tag.
            </video>
            <a href="/public/videos/travel_clip.mp4" class="file-link" download>Download Video</a>
        </div>
        
        <div class="file-item">
            <h2>Document</h2>
            <p>📄 PDF File</p>
            <a href="/public/files/project_report.pdf" class="file-link" download>Download Report (PDF)</a>
        </div>

        <div class="file-item">
            <h2>Another Photo</h2>
            <img src="/public/images/city_view.webp" alt="A city view image">
            <a href="/public/images/city_view.webp" class="file-link" download>Download Image</a>
        </div>

    </div>

    <p style="margin-top: 40px; text-align: center;"><em>The files above must exist at the specified public URLs for this to work.</em></p>

</body>
</html>
