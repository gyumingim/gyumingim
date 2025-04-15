### Language
javascript, Typescript

### FrontEnd
React, Next, Zustand, Axios, StyledComponents, TailwindCss



<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            width: 100%;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            background-color: white;
            overflow: hidden;
            perspective: 1000px;
        }

        .satellites {
            border: 4px solid white;
            transform-style: preserve-3d;
            display: flex;
            justify-content: center;
            align-items: center;
            position: relative;
            width: 300px;
            height: 300px;
            user-select: none;
            cursor: grab;
            animation: rotate 25s linear infinite;
            transform-style: preserve-3d;
        }

        @keyframes rotate {
            from {
                transform: rotateY(0deg);
            }
            to {
                transform: rotateY(360deg);
            }
        }

        .satellite {
            position: absolute;
            width: 200px !important;
            transform: rotateY(calc(var(--i) * 1deg)) translateZ(372px) !important;
            transition: transform 0.2s ease;
            backface-visibility: hidden;
            -webkit-user-drag: none;
            image-rendering: -webkit-optimize-contrast;
            image-rendering: crisp-edges;
            object-fit: contain;
            /* 이미지 비율 유지 */
        }
    </style>
</head>

<body>
    <div class="satellites">
        <img class="satellite" style="--i: 0;" src="https://velog.velcdn.com/images/gyumingim/post/cebfc028-3fa5-4509-9239-95c5337636f5/image.webp" alt="Album image 1" draggable="false">
        <img class="satellite" style="--i: 30;" src="https://velog.velcdn.com/images/gyumingim/post/d0953034-c3f0-41dd-bba8-ec0a70c57090/image.webp" alt="Album image 2" draggable="false">
        <img class="satellite" style="--i: 60;" src="https://velog.velcdn.com/images/gyumingim/post/87e563dd-9a9e-49d3-a9be-68c94040f95c/image.webp" alt="Album image 3" draggable="false">
        <img class="satellite" style="--i: 90;" src="https://velog.velcdn.com/images/gyumingim/post/7fa52640-1ef3-4d50-8a3c-8791140f6e7b/image.webp" alt="Album image 4" draggable="false">
        <img class="satellite" style="--i: 120;" src="https://velog.velcdn.com/images/gyumingim/post/6fc95b20-db40-4a6d-bb5e-ee40b1a0eac4/image.webp" alt="Album image 5" draggable="false">
        <img class="satellite" style="--i: 150;" src="https://velog.velcdn.com/images/gyumingim/post/a40e4cf4-6e9c-4d08-af70-53021544028a/image.webp" alt="Album image 6" draggable="false">
        <img class="satellite" style="--i: 180;" src="https://velog.velcdn.com/images/gyumingim/post/5a9c3f77-870f-4939-891b-322b63ec73ef/image.webp" alt="Album image 7" draggable="false">
        <img class="satellite" style="--i: 210;" src="https://velog.velcdn.com/images/gyumingim/post/1890a354-9510-47d1-9e3a-1a2f6f286618/image.webp" alt="Album image 8" draggable="false">
        <img class="satellite" style="--i: 240;" src="https://velog.velcdn.com/images/gyumingim/post/fe7ecfdf-7175-4a6b-b330-63628430191d/image.webp" alt="Album image 9" draggable="false">
        <img class="satellite" style="--i: 270;" src="https://velog.velcdn.com/images/gyumingim/post/22956517-2b8f-4a4b-961a-57c937796535/image.webp" alt="Album image 10" draggable="false">
        <img class="satellite" style="--i: 300;" src="https://velog.velcdn.com/images/gyumingim/post/674f019a-f69d-442d-8763-b56f74639f97/image.webp" alt="Album image 11" draggable="false">
        <img class="satellite" style="--i: 330;" src="https://velog.velcdn.com/images/gyumingim/post/34783e0b-a9be-46ca-a499-89627d5f8d08/image.webp" alt="Album image 12" draggable="false">
        <img class="satellite" style="--i: 330;" src="https://velog.velcdn.com/images/gyumingim/post/2f385380-a70f-4d24-969c-010e8a27bd57/image.webp" alt="Album image 12" draggable="false">
        <img class="satellite" style="--i: 330;" src="https://velog.velcdn.com/images/gyumingim/post/34036f34-3a9b-4741-9a80-d616259514e1/image.webp" alt="Album image 12" draggable="false">
        <img class="satellite" style="--i: 330;" src="https://velog.velcdn.com/images/gyumingim/post/9be8eef2-109e-49aa-a964-3ae8fe6e2d53/image.webp" alt="Album image 12" draggable="false">
        <img class="satellite" style="--i: 330;" src="https://velog.velcdn.com/images/gyumingim/post/0bd9c4b9-621f-45a8-a129-4e284a351613/image.jpg" alt="Album image 12" draggable="false">
    </div>
</body>
</html>
