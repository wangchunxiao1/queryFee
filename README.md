<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>筛选页面</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f5f5f5;
        }
        .container {
            max-width: 600px;
            margin: 0 auto;
            padding: 20px;
            background-color: #ffffff;
            border-radius: 8px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }
        h1 {
            font-size: 24px;
            margin-bottom: 20px;
        }
        .form-group {
            margin-bottom: 20px;
        }
        .form-group label {
            display: block;
            font-size: 18px;
            margin-bottom: 10px;
        }
        .form-group input,
        .form-group select {
            width: 100%;
            padding: 10px;
            font-size: 16px;
            border: 1px solid #ccc;
            border-radius: 4px;
        }
        .form-group button {
            padding: 10px 20px;
            font-size: 16px;
            border: none;
            border-radius: 4px;
            background-color: #ff9800;
            color: #ffffff;
            cursor: pointer;
        }
        .form-group button:hover {
            background-color: #ff7000;
        }
        .form-group button[type="reset"] {
            background-color: #f44336;
        }
        .form-group button[type="reset"]:hover {
            background-color: #d32f2f;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>筛选</h1>
        <form>
            <div class="form-group">
                <label for="start-date">交易时间</label>
                <input type="date" id="start-date" name="start-date" value="2024-08-22">
                <span>—</span>
                <input type="date" id="end-date" name="end-date" value="2024-08-29">
            </div>
            <div class="form-group">
                <label for="transaction-type">交易类型</label>
                <div>
                    <button type="button">全部</button>
                    <button type="button">收入</button>
                    <button type="button">支出</button>
                </div>
            </div>
            <div class="form-group">
                <label for="amount-range">金额</label>
                <input type="number" id="min-amount" name="min-amount" placeholder="最小金额">
                <span>—</span>
                <input type="number" id="max-amount" name="max-amount" placeholder="最大金额">
            </div>
            <div class="form-group">
                <label for="transaction-summary">交易摘要</label>
                <div>
                    <button type="button">全部</button>
                    <button type="button">工资</button>
                    <button type="button">理财</button>
                    <button type="button">基金</button>
                    <button type="button">外汇</button>
                </div>
            </div>
            <div class="form-group">
                <label for="counterparty-name">交易对方</label>
                <input type="text" id="counterparty-name" name="counterparty-name" placeholder="对方名称">
            </div>
            <div class="form-group">
                <label for="counterparty-account">对方账号（试试输入卡号后四位）</label>
                <input type="text" id="counterparty-account" name="counterparty-account" placeholder="对方账号">
            </div>
            <div class="form-group">
                <button type="reset">重置</button>
                <button type="submit">确定</button>
            </div>
        </form>
    </div>
</body>
</html>
