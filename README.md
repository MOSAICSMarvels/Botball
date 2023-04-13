#include <kipr/create.h>
//Grab the pool noodle with CreateBot






int main()
{
    enable_servos();
    set_servo_position(0,1885);
    set_servo_position(2,1147);
   
    wait_for_light(1);
    shut_down_in(119);
    
    motor(0,75);
    motor(3,75);
    msleep(1500);
    
    ao();
    
    msleep(500);
    
    motor(0,0);
    motor(3,75);
    msleep(1950);
    
    motor(0,75);
    motor(3,75);
    msleep(5200);
    
    motor(0,75);
    motor(3,0);
    msleep(2050);
    
    motor(0,75);
    motor(3,75);
    msleep(2300);
    ao();
    
    set_servo_position(0,1403);
    msleep(1000);
    
    
    set_servo_position(2,1694);
    msleep(1000);
    
    
    motor(0,-75);
    motor(3,-75);
    msleep(3000);
    
    disable_servos();
    
   return 0;
}
