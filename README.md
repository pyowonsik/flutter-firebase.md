# flutter-firebase.md



pubspec.yaml 

  cloud_firestore:
  firebase_core:
  firebase_auth:

추가

1. flutter login
2. firebase projects:create 프로젝트명(영어로)(따음표 없음)
3. dart pub global active flutterfire_cli -> 환경변수 export
4. flutterfire configure

main.dart
void main() async {
  WidgetsFlutterBinding.ensureInitialized();
  await Firebase.initializeApp(
    options: DefaultFirebaseOptions.currentPlatform,
  );
  
추가


- ios 연동 
.list 파일 runnuer 에 추가
.list revered_client_id 복사
target runner url type- url schemas에 붙여넣기
pod init -> install -> flutter run
