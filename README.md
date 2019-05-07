# Gross-Framework-Organized-Views-and-Controls
## For those who want to make it beautiful on the first day of service.
### (The framework is under development)

This structure aims to organize and increase the productivity of the team. The framework separates the viewpoints from the controls, and this saves us time by working with projects where we see a complicated framework to understand and somehow we are stuck in order to adapt to the life cycle of that application.

### Template that will correct
<?php 
....
$Query = "SELECT id, firstname, lastname FROM table";
$result = $conn->query($Query);

if ($result->num_rows > 0) {
    // output data of each row
    while($row = $result->fetch_assoc()) {
        echo "id: " . $row["id"]. " - Name: " . $row["
result-one"]. " " . $row["result-two"]. "<br>";
    }
} else {
    echo "0 results";
}
$conn->close();
...?>

### Organized form
<?php 
...
$Query = "$list-> id, firstname, lastname FROM table";
$result = $conn->query($Query);
if ($result-> 0) {
    // output data of each row
    while($row = $result->fetch_assoc()) {
        echo $viewData;
    }
} else {
    echo "0 results";
}
close_connection();
...?>
