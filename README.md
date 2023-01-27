# secret
            $("#isSecret").click(function(){

                if(this.checked){
                    $("#password").prop("disabled",false);
                }
                else{
                    $("#password").prop("disabled",true);
                }
            });
            
            
            
            CREATE TABLE board3.tc_post (
    `id`            bigint(20)    NOT NULL AUTO_INCREMENT COMMENT 'PK',
    `title`         varchar(100)  NOT NULL COMMENT '제목',
    `content`       varchar(3000) NOT NULL COMMENT '내용',
    `writer`        varchar(20)   NOT NULL COMMENT '작성자',
    `view_cnt`      int(11)       NOT NULL COMMENT '조회 수',
    `secret_yn`     tinyint(1)    NOT NULL COMMENT '비밀글 여부',
    `password`      varchar(100)  NOT NULL COMMENT '비밀번호',
    `delete_yn`     tinyint(1)    NOT NULL COMMENT '삭제 여부',
    `created_date`  datetime      NOT NULL DEFAULT current_timestamp() COMMENT '생성일시',
    `modified_date` datetime               DEFAULT NULL COMMENT '최종 수정일시',
    PRIMARY KEY (`id`)
) COMMENT '게시글';  
            
            
            intellij Debug 모드
