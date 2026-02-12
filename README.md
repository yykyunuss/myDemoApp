this project is about software engineering homework
https://travis-ci.org/yykyunuss/myDemoApp.svg?branch=master
DEMO SITE: https://safe-river-59912.herokuapp.com


import lombok.Getter;
import lombok.Setter;
import lombok.NoArgsConstructor;
import java.util.List;
import java.util.Map;

@Getter
@Setter
@NoArgsConstructor
public class GetUrlWithTokenRequest {
    
    private Long customerNo;
    private Long delegateCustomerNo;
    private Long identityNumber; // zorunlu alan
    private String countryCode; // zorunlu alan
    private String mobilePhoneNo; // zorunlu alan
    private Long taxNumber;
    private String deviceId;
    private String birthDate; // zorunlu alan, dd/MM/yyyy formatı
    private Map<String, DirectionDataDTO> directionData;
    private String externalReference;
    private String channelName;
    private String processType;
    private String processCode;
    private String redirectProcessType;
    private String redirectProcessCode;
    private String redirectScreenName;
    private String redirectUrl;
    private Boolean notifyWithSms;
    private String flowName; // zorunlu alan, DOB_210 veya DOB_205
}


import lombok.Getter;
import lombok.Setter;
import lombok.NoArgsConstructor;

@Getter
@Setter
@NoArgsConstructor
public class DirectionDataDTO {
    private String dataValue;
    private String dataInfo;
}
