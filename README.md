# Radyabnegar-form
html
<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>فرم ثبت اطلاعات</title>
    <style>
        * {
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: #f5f7fa;
            margin: 0;
            padding: 20px;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
        }
        
        .form-container {
            background-color: white;
            border-radius: 10px;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
            padding: 30px;
            width: 100%;
            max-width: 500px;
        }
        
        .form-title {
            color: #2c3e50;
            text-align: center;
            margin-bottom: 25px;
            font-size: 24px;
        }
        
        .form-group {
            margin-bottom: 20px;
        }
        
        label {
            display: block;
            margin-bottom: 8px;
            color: #34495e;
            font-weight: 600;
        }
        
        input, select {
            width: 100%;
            padding: 12px 15px;
            border: 1px solid #ddd;
            border-radius: 6px;
            font-size: 16px;
            transition: border-color 0.3s;
        }
        
        input:focus, select:focus {
            border-color: #3498db;
            outline: none;
            box-shadow: 0 0 0 3px rgba(52, 152, 219, 0.2);
        }
        
        .submit-btn {
            background-color: #3498db;
            color: white;
            border: none;
            padding: 12px 20px;
            width: 100%;
            border-radius: 6px;
            cursor: pointer;
            font-size: 16px;
            font-weight: 600;
            transition: background-color 0.3s;
        }
        
        .submit-btn:hover {
            background-color: #2980b9;
        }
        
        @media (max-width: 600px) {
            .form-container {
                padding: 20px;
            }
        }
    </style>
</head>
<body>
    <div class="form-container">
        <h1 class="form-title">فرم ثبت اطلاعات</h1>
        <form action="/submit" method="POST">
            <div class="form-group">
                <label for="firstName">نام</label>
                <input type="text" id="firstName" name="firstName" placeholder="نام خود را وارد کنید" required>
            </div>
            
            <div class="form-group">
                <label for="lastName">نام خانوادگی</label>
                <input type="text" id="lastName" name="lastName" placeholder="نام خانوادگی خود را وارد کنید" required>
            </div>
            
            <div class="form-group">
                <label for="mobile">شماره موبایل</label>
                <input type="tel" id="mobile" name="mobile" placeholder="09xxxxxxxxx" pattern="09[0-9]{9}" required>
            </div>
            
            <div class="form-group">
                <label for="city">شهر</label>
                <select id="city" name="city" required>
                    <option value="" disabled selected>شهر خود را انتخاب کنید</option>
                    <option value="tehran">تهران</option>
                    <option value="mashhad">مشهد</option>
                    <option value="isfahan">اصفهان</option>
                    <option value="shiraz">شیراز</option>
                    <option value="tabriz">تبریز</option>
                    <option value="other">سایر</option>
                </select>
            </div>
            
            <button type="submit" class="submit-btn">ثبت اطلاعات</button>
        </form>
    </div>
</body>
</html>
```
