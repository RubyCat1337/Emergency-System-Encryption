# Emergency-System-Encryption


# Шифрування системи екстреної допомоги

Скрипт мовою Python для шифрування конфіденційних даних за допомогою алгоритму Advanced Encryption Standard (AES) з ключем довжиною 512 біт. Зашифровані дані зберігаються у файлі, а ключ шифрування зберігається для можливого розшифрування.

## Інструкції з використання

### Вимоги
- Python 3.x
- бібліотека pycryptodome (`pip install pycryptodome`)

### Кроки

1. **Клонування репозиторію:**
   ```bash
   git clone https://github.com/your-username/Emergency-System-Encryption.git
   cd Emergency-System-Encryption


Запуск скрипту шифрування:

Відкрийте файл encrypt_data.py та змініть змінну **file_path**, щоб вказати шлях до файлу, який ви хочете зашифрувати.
    
file_path = "шлях/до/вашого/файлу.txt"
Збережіть зміни та запустіть скрипт:
python encrypt_data.py


Зашифровані дані будуть збережені у файлі, вказаному в скрипті (за замовчуванням - **encrypted_data.bin**), а ключ шифрування буде збережено в **encryption_key.bin**

***Розшифрування (за потреби):***

Для розшифрування даних використовуйте функцію **decrypt** в файлі **decrypt_data.py**. Відредагуйте змінні **encrypted_file_path** та **decrypted_file_path** відповідно і запустіть скрипт.

###Полезная информация

для полного шыврования диска используйте BitLocker и PowerShell

Включите BitLocker на диске C:.
Enable-BitLocker -MountPoint "C:" -EncryptionMethod Aes256 -UsedSpaceOnly

Возможно, вам придется перезагрузить компьютер, чтобы завершить процесс.
Restart-Computer
