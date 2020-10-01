package voc;
import java.util.Scanner;
public class Main {

	public static void main(String[] args) {
		Scanner cin =new Scanner(System.in);
		String [] eng = {"employ","employer","employee","employment","corporation",
				"corporate","suffer","terminal","terminal","illness","ill",
				"tremendously","tremendous","laughter","frighten","fright","contact",
				"contact","contact","germ","warmth","warmth","frail","prompt","prompt"
				,"pale","confine","confine","sparkle","sparkle","hug","hug","drowsy",
				"stretch","stretch","refuse","refusal","hesitate","hesitation","promise",
				"promise","material","mention","structure","capable","capability",
				"collaborate","collaboration","architect","architecture","graduate","graduate"
				,"graduation","construct","construction","construction","constructive",
				"slightly","slight","rank","ranking","unique","innovative","innovate",
				"innovation","adjust","adjustment","rely","reliable","feedback","element",
				"elementary","stability","stable","route","explore","exploration",
				"humankind","universe","universal","fur","fur","enable","upright",
				"upright","generous","generosity","conflict","conflict",
				"distribution","distribute","benefit","benefit","benefit",
				"beneficial","slaughter","slaughter","slaughter","underneath",
				"freeze","freeze","victim","miserable","misery","hollow",
				"furious","fury","theft","punish","punishment","banish",
				"banishment","torture","torture","civilization","artificial",
				"coralreef","ridiculous","layer","electronic","electronic",
				"electricity","equip","equipment","flex","flexible","relatively",
				"relative","relative","temperature","precious","balance",
				"balance","balance","balance","habitat","texture","erect",
				"reduce","reduction","assemble","individual","individual"
		};
		boolean [] judge = new boolean [143];
		int sum=0;
		int n=0;
		while(cin.hasNext() && n !=-1) {
			n=cin.nextInt();
			int random = (int) (Math.random()*142)+1;
			if(!judge[random]) {
				System.out.println(eng[random].charAt(0)+"_____"+eng[random].charAt(eng[random].length()-1));
				int m=cin.nextInt();
				if(m==1) sum++;
				System.out.println(eng[random]);
				judge[random]=true;
			}
			
		}
		System.out.println(sum);
	}

}
