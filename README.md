
 #SMART TRAFIC MANAGEMENT SYSTEM
class TrafficDevice:
    def activate(self):
        print("Traffic management devices activated.")


class TrafficLight(TrafficDevice):
    def activate(self):
        print("Traffic Light: Green light ON.")


class SpeedCamera(TrafficDevice):
    def activate(self):
        print("Speed Camera: Capturing speeding vehicles.")


class PedestrianSignal(TrafficDevice):
    def activate(self):
        print("Pedestrian Signal: No pedestrian is moving.")


class EmergencySiren(TrafficDevice):
    def activate(self):
        print("Emergency Siren: There is an emergency please clear the road.")

#OBJECTS
traffic_light = TrafficLight()
speed_camera = SpeedCamera()
pedestrian_signal = PedestrianSignal()
emergency_siren = EmergencySiren()


devices = [
    traffic_light,
    speed_camera,
    pedestrian_signal,
    emergency_siren
]


for device in devices:
    device.activate()
