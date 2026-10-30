<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Grid Photo Gallery</title>

    <style>
        * {
            box-sizing: border-box;
            margin: 0;
        }

        body {
            font-family: Arial, sans-serif;
            background: #111;
            color: white;
            padding: 20px;
        }

        h1 {
            text-align: center;
            margin-bottom: 20px;
        }

        /* Gallery layout */
        .gallery {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            grid-auto-rows: 180px;
            gap: 10px;
            max-width: 1100px;
            margin: auto;
        }

        /* Image boxes */
        figure {
            position: relative;
            overflow: hidden;
            border-radius: 10px;
        }

        img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            display: block;
            transition: transform 0.4s;
        }

        /* Hover effect */
        figure:hover img {
            transform: scale(1.08);
        }

        /* Image captions */
        figcaption {
            position: absolute;
            bottom: 0;
            left: 0;
            width: 100%;
            padding: 8px;
            background: rgba(0, 0, 0, 0.6);
        }

        /* Different image sizes */
        .wide {
            grid-column: span 2;
        }

        .tall {
            grid-row: span 2;
        }

        .big {
            grid-column: span 2;
            grid-row: span 2;
        }

        /* Tablet screen */
        @media (max-width: 800px) {
            .gallery {
                grid-template-columns: repeat(2, 1fr);
            }
        }

        /* Mobile screen */
        @media (max-width: 480px) {
            .gallery {
                grid-template-columns: 1fr;
            }

            .wide, .big {
                grid-column: auto;
            }
        }
    </style>
</head>

<body>

    <h1>My Gallery</h1>

    <div class="gallery">

        <figure class="big">
            <img src="https://picsum.photos/id/1015/800/800" alt="River valley">
            <figcaption>River Valley</figcaption>
        </figure>

        <figure>
            <img src="https://picsum.photos/id/1016/400/400" alt="Canyon">
            <figcaption>Canyon</figcaption>
        </figure>

        <figure class="tall">
            <img src="https://picsum.photos/id/1018/400/800" alt="Mountain peak">
            <figcaption>Mountain Peak</figcaption>
        </figure>

        <figure>
            <img src="https://picsum.photos/id/1019/400/400" alt="Wooden jetty">
            <figcaption>Wooden Jetty</figcaption>
        </figure>

        <figure class="wide">
            <img src="https://picsum.photos/id/1036/800/400" alt="Winter forest">
            <figcaption>Winter Forest</figcaption>
        </figure>

        <figure>
            <img src="https://picsum.photos/id/1039/400/400" alt="Waterfall">
            <figcaption>Waterfall</figcaption>
        </figure>

        <figure>
            <img src="https://picsum.photos/id/1043/400/400" alt="Evening sky">
            <figcaption>Evening Sky</figcaption>
        </figure>

    </div>

</body>
</html>

