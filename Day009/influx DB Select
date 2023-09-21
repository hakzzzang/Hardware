from influxdb import InfluxDBClient
client = InfluxDBClient(host = '192.168.1.33', port=8086, username='influx_ship', password='1234', database='db_riatech')
results = client.query('select * from sensors')
points = results.get_points()
for point in points:
    print(point)
