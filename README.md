# Encryption-and-Decryption
 prompt={'Enter last name:','Enter first name:','Enter message:'};
title='Encryption Demo';
answer=inputdlg(prompt,title);
lastname=answer{1};
firstname = answer{2};
message= answer{3};

    Choice = questdlg('Want to perform encryption and Decrtyption','Choice Menu','DEFAULT');
switch Choice
   case 'Yes'
       
        action =answer{1};
        message1=double(message);
        message2=((message1+90));
        disp('hello');
        disp(firstname);
        disp(lastname);
        format shortg;
        disp('ENCRYPTION BIGIN');
        disp(message1);
        disp(message2);
        disp('YOUR ENCRYPTED MESSAGE IS');
        message3=char(message2);
        disp(message3);
        disp('DECRYPTION BEGIN');
        disp(message3);
        disp(message2);
        message5=(message2 - 65);
        disp(message5);
        message6=[char(message5)];
        disp('YOUR DECRYPTED MESSAGE IS');
        disp(message6);
            b1 = msgbox(['The Encryptrd Text message is :' message3], 'Encryption Process');
            uiwait(b1);
            b2= msgbox(['your decrypted message is :' message1], 'Decryption Process');
            uiwait(b2);
    case 'No'
           b3 = msgbox('You have wasted my time','Not Interested','warn');
    case 'Cancel'
           b4 = msgbox('NOW YOU CAN NOT PERFORME ENCRYPTION','WARNING','WARN');
 end



