# 19.02.22

   <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <h1>Моя первая страничка</h1>
    <nav id="nav">
        <div class="logo"><a href="/"><img src="" alt="" scr="/images/logo.png"></a></div>
    </nav>
    <div class="menu">
    <a href="index001.html">Пункт001</a>
    <a href="index002.html">Пункт002</a>
    <a href="index003.html">Пункт003</a>
    <a href="index004.html">Пункт004</a>
    <a href="index005.html">Пункт005</a>
</body>
</html>
 <?php
    function nav($item)
    {$items=[
        "index.php" => "Главная"
        "login.php" => "Вход"
        "registr.php" => "Регистрация"
        "admin.php" => "Администрирование"
        "lk.php" => "Личный кабинет"
        "logout.php" => "Выход"

    ];
    echo "<nav>";
    $i = 0 ;
    foreach($items as $key => $value) ; 
{ if($i == $item)
    echo "<a href='$key'class='active>$value</a>";
    else
    echo "<a href='$key'class='active>$value</a>";
    $i++;
}
echo "</nav>";
    }
?>

<?php		
		include 'nav.php';
		nav(2);
		?>
		<div class="register">
		<form action="registeraction.php" class="form" method="POST">
		<input type="text" placeholder="ФИО" name="fio">
		<input type="text" placeholder="логин" name="login">
		<input type="email" placeholder="email" name="email">
		<input type="password" placeholder="пароль" name="password">
		<input type="password" placeholder="еще раз пароль" name="confirm">
		<label><input type="checkbox">Согласие на обработку персональных данных/label>
		<button>Регистрация</button>
		</form>
		</div>
		</body>
		</html


</body>
</html>
