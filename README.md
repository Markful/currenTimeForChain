# currenTimeForChain
public class currentTime {
    public static void main(String[] args) {

        long totalMillisSeconds = System.currentTimeMillis();
        //毫秒转换成秒
        long totalSeconds = totalMillisSeconds / 1000 ;
        //得到现在的秒数单位
        long currentSeconds = totalSeconds % 60;
        //得到总的分钟数
        long totalMinutes = totalSeconds / 60;
        //得到现在的分钟数
        long currentMinutes = totalMinutes % 60;

        long totalHours = totalMinutes / 60;

        long currentHours = totalHours % 24;
        //出来的会是美国时间，需要加8变成北京时间
        System.out.println("Current Time Is " + (currentHours + 8) + ":" + currentMinutes + ":" +currentSeconds );
    }
}
