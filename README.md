# WebApp1
from flask import Flask ,render_template

app=Flask(__name__)

@app.route('/')
@app.route("/Home")
def Home():
    return "<h1> Home Page </h1>"

@app.route('/About')
def About():
    return "<h2> About Page </h2>"


if __name__ == '__main__':
    app.run(debug=True)
