# Analysis-of-user-activity-in-Google-Spreadsheets
The analysis of user activity in Google Spreadsheets involves statistical calculations, chart creation, data modifications, cohort analysis, and user retention, aiming to better understand and optimize user interactions on the platform.

# Analiza aktywności użytkowników w Google Spreadsheets dla GitHub

## Spis treści
1. [Opis zadania](#opis-zadania)
2. [Description](#description)

---

## Opis zadania

### Obliczenia w zakładce "active users":
1. **Średni wiek**
2. **Odchylenie standardowe (Standard deviation)**
3. **Mediana**
4. **Rozstęp międzykwartylowy (Іnterquartile range)**
5. **10 percentyl wieku**
6. **90 percentyl wieku**
7. **Obliczenie DAU, WAU oraz stickiness użytkowników**
8. **Oszacowanie DAU i WAU dla nadchodzących tygodni**

### Wykresy:
1. Wykres z danymi ze strony "active users". Typu poziomy bar chart pokazujący liczbę użytkowników dla każdego language.
2. Wykres z danymi ze strony "active users". Typu pie chart, który pokazuje podział użytkowników według has_older_device_model.
3. Wykres z danymi ze strony "WAU", który zawiera tygodnie na osi poziomej i dwie osie pionowe: WAU i DAU/WAU. WAU wizualizowane za pomocą słupków, a DAU/WAU za pomocą linii.
4. Wykres z danymi ze strony "WAU", z tygodniami na osi poziomej i wartościami WAU na osi pionowej. Z wielomianową trend line do tego wykresu w potędze 3.

### Modyfikacje w arkuszu "activity":
1. Podział kolumny game_activity_name na dwie części: nazwę gry i nazwę aktywności.
2. Połączenie 8 nazw aktywności w 5 typów aktywności i wyświetlenie typu aktywności w osobnej kolumnie w arkuszu "activity".

### Dodatkowe działania w arkuszu "activity":
1. Utworzenie kolumny z językiem użytkownika i wypełnienie jej danymi z arkusza "active users".
2. Utworzenie trzech kolumn na podstawie kolumny activity_date: 
   a. Activity month - miesiąc aktywności, tj. miesiąc zawierający activity_date.
   b. First activity month - pierwszy miesiąc aktywności dla każdego użytkownika.
   c. Activity month number - liczba reprezentująca miesiąc aktywności.

### Analiza kohortowa:
1. Utworzenie nowego arkusza "Cohort analysis" z tabelą przestawną, która wykorzystuje dane z arkusza "activity".
2. Zwizualizowanie liczby użytkowników w każdym miesiącu aktywności. Utwórzenie line chart z osią poziomą - Activity month number i osią pionową — liczba użytkowników, którzy mają odpowiedni month number.
3. Utworzenie pivot table w osobnym arkuszu, wykorzystująca dane z arkusza "activity".

### Retencja użytkowników:
1. Utworzenie tabeli wyświetlającej retention rate użytkowników.
2. Zastosowanie conditional formatting do obu tabel, aby wyróżnić najwyższe i najniższe wartości.

### Fragmentacja danych:
1. Dodanie trzech fragmentów: nazwa gry, typ aktywności i język użytkownika.

---

## Description

### Calculations in the "active users" tab:
1. **Average age**
2. **Standard deviation**
3. **Median**
4. **Interquartile range**
5. **10th percentile of age**
6. **90th percentile of age**
7. **Calculation of DAU, WAU, and user stickiness**
8. **Estimation of DAU and WAU for upcoming weeks**

### Charts:
1. Horizontal bar chart showing the number of users for each language from the "active users" page.
2. Pie chart showing the distribution of users by has_older_device_model from the "active users" page.
3. Chart with data from the "WAU" page, containing weeks on the horizontal axis and two vertical axes: WAU and DAU/WAU. WAU visualized using bars, and DAU/WAU using lines.
4. Chart with data from the "WAU" page, with weeks on the horizontal axis and WAU values on the vertical axis. Polynomial trend line of power 3 to this chart.

### Modifications in the "activity" sheet:
1. Splitting the game_activity_name column into two parts: game name and activity name.
2. Combining 8 activity names into 5 activity types and displaying the activity type in a separate column in the "activity" sheet.

### Additional actions in the "activity" sheet:
1. Creating a column with the user's language and filling it with data from the "active users" sheet.
2. Creating three columns based on the activity_date column:
   a. Activity month - the month of activity, i.e., the month containing the activity_date.
   b. First activity month - the first month of activity for each user.
   c. Activity month number - a number representing the month of activity.

### Cohort Analysis:
1. Creating a new "Cohort analysis" sheet with a pivot table that utilizes data from the "activity" sheet.
2. Visualizing the number of users in each activity month. Creating a line chart with the horizontal axis being Activity month number and the vertical axis being the number of users who have the respective month number.
3. Creating a pivot table in a separate sheet, utilizing data from the "activity" sheet.

### User Retention:
1. Creating a table displaying the retention rate of users.
2. Applying conditional formatting to both tables to highlight the highest and lowest values.

### Data Fragmentation:
1. Adding three fragments: game name, activity type, and user language.
