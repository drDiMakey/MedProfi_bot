# MedProfi_bot
Телеграмм-бот для частного мед центра
виртуальный ассистент клиники «Мед-Профи». 
Я помогаю с информацией о наших услугах, ценах, записи на прием и другими вопросами, связанными с медицинским обслуживанием. 
Использовали сервисы:
Qwen и GigaChat - для создания системного промпта и базы знаний.
Савви https://suvvy.ai/ - для создания ИИ-ассистента.
Иллюстрации
https://private-user-images.githubusercontent.com/206894699/431909370-be4a42f6-5041-4485-acda-9b86f91fa617.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NDQyMTIxNDAsIm5iZiI6MTc0NDIxMTg0MCwicGF0aCI6Ii8yMDY4OTQ2OTkvNDMxOTA5MzcwLWJlNGE0MmY2LTUwNDEtNDQ4NS1hY2RhLTliODZmOTFmYTYxNy5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUwNDA5JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MDQwOVQxNTE3MjBaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT04ODdjMmM2MDY2MTcxZmJlMmQwNGUwZDUxODcwYzlhYTg4Mjk4NGU5YTJhMjU2NjA4MzY1ZTMyYjQ3YjNiZmFhJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.CEZ1Pdz8TnP4mszNJFDUOVKp9fllf0j_PEKjYK-LCwc
https://private-user-images.githubusercontent.com/206894699/431909370-be4a42f6-5041-4485-acda-9b86f91fa617.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NDQyMTIyMzEsIm5iZiI6MTc0NDIxMTkzMSwicGF0aCI6Ii8yMDY4OTQ2OTkvNDMxOTA5MzcwLWJlNGE0MmY2LTUwNDEtNDQ4NS1hY2RhLTliODZmOTFmYTYxNy5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUwNDA5JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MDQwOVQxNTE4NTFaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1hZTlmMTAwZjA5ODBlNzU4MzdmZTZiZTEzYzhhMGYyYjZiOTc2ZWMxZGViYjhhZTczNmZiZjQwZWExNTQ0NzA2JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.xjs4DZIKQ4VLANNhOZA7Jav_rjVLCVw4pp2avFV2zh8@MedProfi73_bot
(https://private-user-images.githubusercontent.com/206894699/431909365-7f584f84-2618-4973-a3e2-de4f77c7da83.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NDQyMTIzMDIsIm5iZiI6MTc0NDIxMjAwMiwicGF0aCI6Ii8yMDY4OTQ2OTkvNDMxOTA5MzY1LTdmNTg0Zjg0LTI2MTgtNDk3My1hM2UyLWRlNGY3N2M3ZGE4My5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUwNDA5JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MDQwOVQxNTIwMDJaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT0yMWE5ODBjNGVhZDg5N2IxNDM1NTk4NmE2OGE1YzhlMmZlZTA0ODU0MzNiZDY1OWVlMzI5OWEzZmU2ZDA0OTg1JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.IHzxKPQzz9dkWlNRFRXPMUJDFbNRPOVMU4c0RGEhWeU)
(https://private-user-images.githubusercontent.com/206894699/431909362-795f9440-c54a-4d0d-a21d-c3a480421892.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NDQyMTIzNTQsIm5iZiI6MTc0NDIxMjA1NCwicGF0aCI6Ii8yMDY4OTQ2OTkvNDMxOTA5MzYyLTc5NWY5NDQwLWM1NGEtNGQwZC1hMjFkLWMzYTQ4MDQyMTg5Mi5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUwNDA5JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MDQwOVQxNTIwNTRaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT0wMTk0MWVmNTQ1ZmQ4OTYxOTAxMzU1YmM1NDFjMmZjZGQzMWNlNTYyMTE4NzdiYmQwMzczN2U2YTA5OTNkYzFhJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.q4ys1FdUflMaotXq6M_6LX7TzxjsYkJburaKGJ5Vf4g)
(https://private-user-images.githubusercontent.com/206894699/431909360-d95fd7d4-aa79-4b40-a183-7e75aa17c2a8.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NDQyMTI0MjIsIm5iZiI6MTc0NDIxMjEyMiwicGF0aCI6Ii8yMDY4OTQ2OTkvNDMxOTA5MzYwLWQ5NWZkN2Q0LWFhNzktNGI0MC1hMTgzLTdlNzVhYTE3YzJhOC5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUwNDA5JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MDQwOVQxNTIyMDJaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT00ZGQyYTRiN2RhNjMwYWEzODUxMWYxMjBlNDc2YmQzMzRjNzA3NmQ1ZGNkZjdhNDA4NDNmNDFkNGM4ZTBkYzg0JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.Pma5o-NlxyooUTBF4nSuu-H8sEZ1o1b0-v1tAXjQiAs)
https://t.me/MedProfi73_bot
