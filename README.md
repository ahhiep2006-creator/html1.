<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Responsive Web Design Project</title>
    <style>
       
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            padding: 20px;
            background-color: #f5f5f5;
        }
        
        h1 {
            text-align: center;
            margin-bottom: 30px;
            color: #333;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
        }
        
       
        .box {
            width: 100%;
            background-color: white;
            border-radius: 8px;
            padding: 20px;
            margin-bottom: 20px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            text-align: center;
        }
        
        .box img {
            width: 100%;
            height: auto;
            border-radius: 4px;
            margin-top: 15px;
        }
        
        
        @media (min-width: 772px) {
            .box {
                width: 45%;
                display: inline-block;
                margin: 2.5%;
                vertical-align: top;
            }
            
            .box img {
                max-height: 30vh;
                object-fit: cover;
            }
        }
        
       
        @media (min-width: 998px) {
            .box {
                width: 30%;
                margin: 1.66%;
            }
        }
        
      
        .info {
            background-color: #e9f7fe;
            padding: 15px;
            border-radius: 8px;
            margin-top: 30px;
        }
        
        .info h2 {
            color: #0066cc;
            margin-bottom: 10px;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Responsive Web Design Project</h1>
        
        <div class="box">
            <h2>Box 1</h2>
            <p>Nội dung của box thứ nhất. Trên mobile, box này sẽ chiếm toàn bộ chiều rộng.</p>
            <img src="https://via.placeholder.com/400x200/4CAF50/FFFFFF?text=Mobile+View" alt="Placeholder Image">
        </div>
        
        <div class="box">
            <h2>Box 2</h2>
            <p>Nội dung của box thứ hai. Trên tablet, box này sẽ chiếm 45% chiều rộng và xếp thành 2 cột.</p>
            <img src="https://via.placeholder.com/400x200/2196F3/FFFFFF?text=Tablet+View" alt="Placeholder Image">
        </div>
        
        <div class="box">
            <h2>Box 3</h2>
            <p>Nội dung của box thứ ba. Trên desktop, box này sẽ chiếm 30% chiều rộng và xếp thành 3 cột.</p>
            <img src="https://via.placeholder.com/400x200/FF9800/FFFFFF?text=Desktop+View" alt="Placeholder Image">
        </div>
        
        <div class="info">
            <h2>Hướng dẫn sử dụng</h2>
            <p>Thay đổi kích thước cửa sổ trình duyệt để xem hiệu ứng responsive:</p>
            <ul>
                <li><strong>Mobile:</strong> Dưới 772px - Một cột duy nhất</li>
                <li><strong>Tablet:</strong> Từ 772px đến 997px - Hai cột ngang</li>
                <li><strong>Desktop:</strong> Trên 998px - Ba cột ngang</li>
            </ul>
        </div>
    </div>
</body>
</html>
