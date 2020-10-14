FROM  conda/miniconda3

WORKDIR /code

RUN conda install -y -c conda-forge scikit-learn pandas joblib flask

COPY app.py .
COPY iris_classifier.joblib .
COPY iris_classifier_features.joblib .

EXPOSE 5080

ENTRYPOINT ["python"]
CMD ["app.py"]
