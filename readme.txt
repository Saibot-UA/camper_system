���������:

�� ���� include
#include <camper>

� OnGameModeInit ����� ����������� � ��
Camper_SetMysqlConnectionHandle(/*���������� ��� �����������*/); //�������� dbHandle


� ����� ����� OnPlayerSpawn ���������:
OnPlayerSpawnCamper(playerid);

� ����� ����


//������
stock camper_GetPlayerMoney(playerid)
    return PlayerInfo[playerid][pMoney]; //PlayerInfo[playerid][pMoney] ������ �� ����

stock camper_SetPlayerMoney(playerid, cmp_money)
{
    PlayerInfo[playerid][pMoney] += cmp_money; //PlayerInfo[playerid][pMoney] ������ �� ����
}

//����
stock camper_GetPlayerMats(playerid)
    return PlayerInfo[playerid][pMats]; //PlayerInfo[playerid][pMats] ������ �� ����

stock camper_SetPlayerMats(playerid, cmp_mats)
{
    layerInfo[playerid][pMats] += cmp_mats; //PlayerInfo[playerid][pMats] ������ �� ����
}

//���������
stock camper_GetPlayerDrugs(playerid)
    return PlayerInfo[playerid][pDrugs]; //PlayerInfo[playerid][pDrugs] ������ �� ����

stock camper_SetPlayerDrugs(playerid, cmp_drugs, bool: cmp_action)
{
    PlayerInfo[playerid][pDrugs] += cmp_drugs; //PlayerInfo[playerid][pDrugs] ������ �� ����
}