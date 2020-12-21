# WebApp1
from flask import Flask ,render_template

app=Flask(__name__)

@app.route('/')
@app.route("/Home")
def Home():
    return render_template('Homepage.html')

@app.route('/About')
def About():
    return render_template('Homepage.html')


if __name__ == '__main__':
    app.run(debug=True)
