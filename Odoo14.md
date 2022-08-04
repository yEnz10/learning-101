python 3.7+
install : Build Tools for Visual Studio
install : postgresql

git clone https://github.com/odoo/odoo.git odoo14_2 --depth=1 -b 14.0

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
