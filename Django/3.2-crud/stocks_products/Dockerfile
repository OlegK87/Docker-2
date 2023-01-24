FROM python:3.10

WORKDIR /Django/3.2-crud/stocks_products

COPY . /Django/3.2-crud/stocks_products

RUN pip install -r /Django/3.2-crud/stocks_products/requirements.txt

ENV SECRET_KEY django-insecure-nw^y+m^wmxza1asgk+)!ua2qx9)g+#v=6%76-9i8i(6eqiw94j
ENV DEBUG 1

RUN python manage.py migrate

CMD ["gunicorn", "--bind", "0.0.0.0:8000", "stocks_products.wsgi"]