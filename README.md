# Android-NetStat

Included in WiDefend Android


try {
            Process p = Runtime.getRuntime().exec("netstat -nputw");
            BufferedReader in = new BufferedReader(new InputStreamReader(p.getInputStream()));
            String line = null;
            while ((line = in.readLine()) != null) {
                tx1.append(line+"\n");
            }
        } catch (IOException e) {
        }
