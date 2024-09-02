class Car { 
  String make;
  String model;
  int year;
  double mileage;   
  Car({
    required this.make,
    required this.model,
    required this.year,
    required this.mileage,
  });
  void drive(double distance) {
    mileage += distance;
  }  
  String displayInfo() {
    return 'Make: $make\nModel: $model\nYear: $year\nMileage: $mileage';
  }
}  
void main() {  
  Car myCar = Car(
    make: 'LUTUS',
    model: 'V8',
    year: 2023,
    mileage: 15000.5,
  );     
  myCar.drive(250.0);   
  print(myCar.displayInfo());
} 
