# Microservices vs. Monolithic architecture

![Microservices vs. monolithic architecture](https://blog.sparkfabrik.com/hubfs/Blog/monolothic-microservices-image-articles.png)

## Monolithic architecture гэж юу вэ?

Monolithic architecture нь бусад application-аас хараат бус, бие даасан, нэгдсэн нэгж хэлбэрээр хөгжүүлэгддэг програм хангамжийн уламжлалт загвар юм. Энэ нь бизнесийн бүх асуудлыг нэгтгэсэн нэг кодын суурьтай, ганц бие, том тооцоолох сүлжээ юм. Энэ төрлийн програмд ​​өөрчлөлт оруулахын тулд кодын суурь руу нэвтэрч, service-side interface-ийн шинэчилсэн хувилбарыг бүтээж, байршуулах замаар стекийг бүхэлд нь шинэчлэх шаардлагатай. Энэ нь шинэчлэлтийг хязгаарлаж, цаг хугацаа их шаарддаг болгодог.

### Monolithic architecture давуу тал

- Simple to develop and test:
  - Бүх бүрэлдэхүүн хэсэг нь нэг кодын санд байдаг тул програмыг хөгжүүлж, турших нь илүү хялбар байдаг.
- Easy to deploy:
  - Аппликейшн нь нэг нэгж учраас байршуулалт нь микро үйлчилгээтэй харьцуулахад харьцангуй хялбар байдаг.
- High performance:
  - Монолит програмууд нь нэг машин дээр байрлуулсан тул гүйцэтгэлийн хувьд маш оновчтой байх боломжтой.
- Easy to scale:
  - RAM, CPU эсвэл хадгалах сан гэх мэт нэмэлт нөөцийг нэмснээр өргөжүүлэлтийг хялбархан хийж болно.

### Monolithic architecture сул тал

- Hard to maintain:
  - Аппликешны хэмжээ, нарийн төвөгтэй байдал өсөх тусам кодын санд засвар хийх, өөрчлөлт оруулахад хэцүү болж магадгүй юм.
- Limited scalability:
  - Зөвхөн нэг хэсгийг өргөжүүлэхийн тулд бүхэл програмд ​​илүү их нөөц нэмэх шаардлагатай болдог.
- Coupled architecture:
  - Бүх component-үүд нь хоорондоо нягт уялдаатай байдаг бөгөөд энэ нь нэг component дээр бусдад нөлөөлөхгүйгээр өөрчлөлт хийхэд хэцүү болгодог.
- Longer development cycles:
  - Шинэ feature болон өөрчлөлт нь програмыг бүхэлд нь дахин compile болон deploy хийх шаардлагатай болгодог. Ингэснээр цаг их зарцуулахаас гадна хөгжүүлэлтийн явцыг удаашруулдаг.

### Monolithic architecture-т хамгийн түгээмэл хэрэглэгддэг стекүүд:

- <img src="https://cdn-icons-png.flaticon.com/512/226/226777.png" height="30"> Java
- <img src="https://avatars.githubusercontent.com/u/4223" height="30"> Ruby on Rails
- <img src="https://static.djangoproject.com/img/logos/django-logo-negative.1d528e2cb5fb.png" height="30"> Django
- <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/7/7d/Microsoft_.NET_logo.svg/1200px-Microsoft_.NET_logo.svg.png" height="30"> .NET

## Microservices architecture гэж юу вэ?

Энэ нь бие даан байршуулах боломжтой хэд хэдэн service-д тулгуурладаг архитектурын арга юм. Эдгээр service-үүд нь тодорхой зорилготой бизнесийн логик, database-тай байдаг. Шинэчлэх, турших, өргөтгөх, deploy хийх зэрэг нь service тус бүр дээр хийгддэг. Microservices нь томоохон бизнес, домэйнтэй холбоотой асуудлуудыг тусдаа, бие даасан кодын суурь болгон салгадаг. Мөн нарийн төвөгтэй байдлыг бууруулдаггүй ч даалгавруудыг бие биенээсээ хамааралгүй үйл ажиллагаа явуулдаг жижиг процессуудад хуваах замаар аливаа нарийн төвөгтэй байдлыг харагдахуйц, удирдах боломжтой болгодог. Microservices-г нэвтрүүлэх нь ихэвчлэн DevOps-тэй хамт явагддаг. Эдгээр нь багууд хэрэглэгчийн шаардлагад хурдан дасан зохицож, тасралтгүй хүргэх боломжийг олгодог.

### Microservices architecture давуу тал

- Scalability:
  - Service бүрийг бие даан томруулж болох бөгөөд энэ нь илүү сайн гүйцэтгэл, илүү хүртээмжтэй байх боломжийг олгодог.
- Flexibility:
  - Service бүрийг бие даан шинэчилж, гаргах боломжтой тул Microservices нь шинэ функцуудыг илүү хурдан хөгжүүлж, ашиглах боломжийг олгодог.
- Resilience:
  - Хэрэв нэг service амжилтгүй болвол бусад service-үүд үргэлжлүүлэн ажиллах боломжтой тул энэ нь бүх програмд ​​нөлөөлөхгүй.
- Technology diversity:
  - Service бүр өөр өөр технологийн стекийг ашиглах боломжтой бөгөөд энэ нь тодорхой ажил тус бүрийн хамгийн сайн хэрэгслийг сонгоход илүү уян хатан байх боломжийг олгодог.

### Microservices architecture сул тал

- Complexity:
  - Олон service-г удирдахад төвөгтэй байдал нь нэмэлт дэд бүтэц, хяналт, менежментийн хэрэгсэл шаарддаг тул хүндрэлтэй байж болно.
- Communication overhead:
  - Service-үүд хоорондоо харилцах шаардлагатай бөгөөд энэ нь програмд ​​нэмэлт зардал, төвөгтэй байдлыг бий болгодог.
- Testing:
  - Туршилт нь service бүрийг тусад нь турших, мөн service хоорондын харилцан үйлчлэлийг шалгах шаардлагатай тул илүү төвөгтэй болж магадгүй юм.
- Security:
  - Олон үйлчилгээг хамгаалах нь цул програмыг хамгаалахаас илүү хэцүү байж болно.

### Microservices architecture-т хамгийн түгээмэл хэрэглэгддэг стекүүд:

- <img src="https://res.cloudinary.com/startup-grind/image/upload/c_fill,dpr_2.0,f_auto,g_center,h_1080,q_100,w_1080/v1/gcs/platform-data-dsc/events/spring-boot-1_5zDxm9B.jpg" height="30"> Spring Boot
- <img src="https://nglogic.com/wp-content/uploads/2022/11/nodejs-1-logo.png" height="30"> Node.js
- <img src="https://miro.medium.com/v2/resize:fit:600/0*6fwIAzIFfrGStZIS.png" height="30"> Kubernetes
