```js
class Marclyn {
  constructor(...options) {
    this.height = "1.78"
    this.weight = "56"
    this.type = "human"
    this.job = "student"
    this.sex = "male"
  }
}

class CreateMan extends Marclyn {
  constructor(...options) {
    super(options);
  }
  
  private _eating() {
    void "eating 🍔 🍟 🍗 🥤"
  }
  
  private _coding() {
    void "coding... ❤️"
  }
  
  private _sleep(ms) { return new Promise(resolve => setTimeout(resolve, ms)) }
  
  async createDay() {
    this._eating()
    this._coding()
    await this._sleep(18000000)
    
    this.createDay()
  }
  
}

let Marclyn = new CreateMan()
Marclyn.createDay();
```
