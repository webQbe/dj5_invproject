# Django Inventory Management App

This is a small and focused Django inventory-management app that demonstrates a complete CRUD workflow for products using **function-based views** and **ModelForms**.

## About
This repo is an adaptation of [Complete Django Tutorial](https://www.youtube.com/playlist?list=PL4cUxeGkcC9iqfAag3a_BKEX1N43uJutw) by Bek Brace. 

I followed the tutorial to learn followings:
* Show the practical use of Django `models`, `forms.ModelForm`, and `views` to implement real features.
* Demonstrate **server-side form handling**, **validation** *(e.g., unique SKU enforced at the model level)*, and **clean redirects** after POSTs.
* Include **Bootstrap classes** in widgets, so the UI can be styled quickly for a polished look.


## How to run (dev)
1. `git clone https://github.com/webQbe/dj5_invproject.git`
2. `python -m venv .venv && source .venv/bin/activate`
3. `pip install -r requirements.txt`
4. `python manage.py migrate && python manage.py createsuperuser`
5. `python manage.py runserver`
---
Then open your browser and go to:
👉 **[http://127.0.0.1:8000/](http://127.0.0.1:8000/)**


## Credits
Original tutorial: [Complete Django Tutorial](https://www.youtube.com/playlist?list=PL4cUxeGkcC9iqfAag3a_BKEX1N43uJutw) — Net Ninja

## License
MIT License






