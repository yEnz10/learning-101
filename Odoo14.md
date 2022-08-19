python 3.7+
install : Build Tools for Visual Studio
install : postgresql

git clone https://github.com/odoo/odoo.git <folder_name> --depth=1 -b 14.0

https://speedysense.com/odoo-module-structure/

```cmd
pip install setuptools wheel

pip install -r requirements.txt

python -m pip install --upgrade pip

python odoo-bin --stop-after-init -s -c .\odoo.conf

python odoo-bin -d <db> -r <user_db> -w <pw_db>
```


### requirements
```py
libsass==0.21.0
passlib==1.7.2
python-stdnum==1.16
```


wkhtmltopdf for Windows:
1. First, download and install wkhtmltopdf for your version of windows (32 bit or 64 bit).
2. Once it's installed, go to Openerp/odoo and go to Settings> Users and click on your user
3. Click edit and scroll down and look for "Technical Features" is enabled / checked.
4. Click Apply, then log out of Odoo and then login
5. Go to Settings again and now you should see several new technical menu items on the left
6. Go to Settings -> Customization -> Parameters -> System Parameters
7. Click Add and for Key insert : webkit_path
8. For value insert: C:\Progra~1\wkhtmltopdf\bin\wkhtmltopdf.exe
9. Apply and exit and restart Windows.
10. After you do the above steps, go to System  in Control Panel.
11. Click on Advanced Settings. The System Properties window will pop up.
12. In the "Advanced" Tab, Click on "Environment Variables". 
13. In the "System variables", scroll down until you find the "Path" variable and double click. !!!!!NOT user variables
14. inside the "Variable value" field, add this to the end: ;C:\Program Files\wkhtmltopdf\bin
15. Click OK and then reboot your system.
