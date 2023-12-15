```dart
    class Camera {
      // _ repersent private in dart
      String? _name;
      String? _color;
      int? _megpix;
      
      Camera(String name,String color,int megpix){
        _name = name;
        _color = color;
        _megpix = megpix;
      }
      // change value by Setter
      set setPix(pix){
         _megpix =pix;
      }
      // get the the value by Getter.
      get getPix {
        return _megpix;
      }

      void display() {
          print("Name: $_name");
          print("Color: $_color");
          print("Current quality: $_megpix MP");
      }
    }

    void main(){
        // Here camera is object of the class Camera. 
        Camera camera=  Camera( 'Samsung a12','multicolor',32 );
        camera.display();
        print('Current quality from Getter: ${camera.getPix} MP \n');
        camera.setPix= 48;
        print('After updating: ');
        camera.display();


    }
```
