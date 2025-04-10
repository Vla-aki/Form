<!DOCTYPE html>
<html lang="hu">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Javascript - Úrlapkezelés</title>
    <style>
        .form-container
        {
            width: 400px;
            margin-left:auto;
            margin-right: auto;
            margin-top: 50px;
        }
        table, td, th
        {
            border: 1px solid black;
            border-collapse: collapse;
            padding: 5px 10px;
        }
    </style>
</head>
<body>
    <div class="form-container">
    <fieldset>
        <legend>Űrlap</legend>
        <form action="" id="userForm">
        <p>
            <label for="vezeteknev">Vezetéknév:</label>
            <input type="text" name="vezeteknev" placeholder="Vezetéknév megadása..">
        </p>
        <p>
            <label for="keresztnev">Keresztnév:</label>
            <input type="text" name="keresztnev" placeholder="Keresztnév megadása..">
        </p>
        <p>
            <label for="email">Email cím:</label>
            <input type="email" name="email" placeholder="Email cím megadása..">
        </p>
        <p>
            <label for="telefonszam">Telefonszám:</label>
            <input type="tel" name="telefonszam" placeholder="Telefonszám megadása..">
        </p>
    </fieldset>
    <p>
        <button type="submit">Elküld</button>
    </p>
        </form>
    <h3>LocalStorage adatok megjelenítése</h3>
    <table>
        <thead>
            <tr>
                <th>Vezetéknév</th>
                <th>Keresztnév</th>
                <th>Email cím</th>
                <th>Telefonszám</th>
            </tr>
        </thead>
        <tbody id="usersTable"><!--Ide jönnek az adatok--></tbody>
    </table>
    </div>
    <script src="form.js"></script>
</body>
</html>
