RecognizeMessageEventContent
=============================

.. code-block:: c#

	class RecognizeMessageEventContent {
		OutboxMessageMeta: OutboxMessageMeta,
		DocumentType: DocumentType,
		SenderPartyId: string,
		RecipientPartyId: string
	}
	
Информация о новом событии - разборе исходящего сообщения и успешном определении его основных параметров (формат, тип, отправитель и получатель). Соответствует BoxEventType = RecognizeMessage.

 - OutboxMessageMeta – :doc:`метаинформация <../../structures/OutboxMessageMeta>` сообщения.
 - DocumentType – :doc:`тип <../../enums/DocumentType>` сообщения.
 - SenderPartyId – отправитель сообщения.
 - RecipientPartyId – получатель сообщения.