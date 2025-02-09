# IBMileKodluyoruz

# Noktaların Tanımlanması:
points=[(3,5),(4,12),(9,6),(8,2)]

# Öklid Mesafesi İçin Bir Fonksiyon Yazma:
def euclideanDistance(point1,point2):
  x1,y1 = point1
  x2,y2 = point2
  return ((x2-x1)**2 + (y2-y1)**2)**0.5

# Mesafelerin Hesaplanması:
distances=[]
for i in range(len(points)):
  for j in range(i+1,len(points)):
    p=euclideanDistance(points[i],points[j])
    distances.append(p)

# Minimum Mesafenin Bulunması:
min_distance=min(distances)

print("Noktalar: ",points)
print("Mesafeler: ",distances)
print("Min mesafe: ",min_distance)
