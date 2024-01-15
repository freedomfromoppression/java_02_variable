# java_02_variable
package ch02_variable;

public class AariableName {

	public static void main(String[] args) {
		// 변수명, 클래스명 명명 규칙

		// 여러줄 주석
		/*
		 * 프로젝트,클래스명 이름은 앞에 대문자를 씀.(JavaStudy..)
		 * 
		 * 패키지(폴더) 이름은 전부 소문자로 작성 필요하다면 단어 사이에 언더바(__)를 넣어서 사용(cha01_start..)
		 * 
		 * 변수명 (or 함수명) 카멜 표기법(Came1, 낙타 표기법이라함.) 첫 글자는 소문자, 다음 단어들은 대문자로 시작 ex)
		 * todayIsHappy
		 * 
		 * python은 스네이크 표기법사용 ex) today_is_happy
		 * 
		 * 
		 */
		// [데이터 타임] [변수명]
		int todayIsHappy = 0;
		System.out.println(todayIsHappy);
		byte byteVar = 1;
		System.out.println(byteVar);
		int intVar = 3;
		System.out.println(intVar);
		long longVar = 3000000000L; // Long 은 L이 붙음
		System.out.println(longVar);
		char charVar = 44032; // "가"와 같음
		System.out.println(charVar);
		// 정수 이면서 문자에 해당
		short shortVar = 2;
		System.out.println(shortVar);
		// 정수 이면서 문자에 해당
		char ga = '가';
		// 소수 타임
		float floatVar = 3.14f;
		System.out.println(floatVar);
		double doubleVar = 3.14f;

		// 불리언 타임(참/거짓, ture/false)
		boolean boolVar = false;

		// 문자열 타입

	}

}
package ch02_variable;

public class VariableMain {
	
	public static void main(String[] args) {
		//상수(Constant) 변경 불가
		final double MATH_PI = 3.14;
//      MATH_PI = 4.23;  // 오류남(상수는 변경이 안되기 때문)
		double mathPi2 = 3.11;
		mathPi2 = 3.14; //변수는 변경가능
		
		//문자열 String 타입은 클래스로 관리되어짐.(다양한 메소드를(함수)를 내장하고 있음)
		String fruits="Apple, Banana, Cherry";
		//.length() 문자열의 길이를 리턴
		System.out.println(fruits);
		System.out.println("길이:"+fruits.length()); //함수는 함수명() <__실행
		//.charAt(안덱스)
		System.out.println("3인덱스:"+fruits.charAt(3));
		//.index0f(문자열)
		//해당 String에서 '문자열'을 찾아서 첫번째 인덱스를 반환 존재하지 않으면 -1반환
		System.out.println("Banana 시작인덱스;"+fruits.indexOf("Banana"));
		//.substring(시작 인덱스) 해당 문자열의 시작 인덱스 부터 끝까지 자른다.
		//.substring(시작,종료인덱스) 해당 문자열의 시작 인덱스부터 끝인덱스 전까지 자른다.
		System.out.println(fruits.substring(15));
		System.out.println(fruits.substring(7,13));
		//.replace(바뀔 문자열, 바꿀 문자열)
		System.out.println(fruits.replace("Cherry","Chamwui"));
		//, <--를 찾아서 로 변경하시오
		System.out.println(fruits.replace(",","|"));
		
		String email="leeapgil@gmail.com";
		//다음 문자열에서 @를 기준으로 앞과 뒤를 각각 출력하시오
		//leeapgil
		//gmail.com
		System.out.println(email.substring(0,8));
		System.out.println(email.substring(9));
		
		
		
		
		
	
	}
	
	
}

    

